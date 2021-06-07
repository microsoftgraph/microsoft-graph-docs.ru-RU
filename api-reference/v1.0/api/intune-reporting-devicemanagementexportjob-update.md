---
title: Обновление deviceManagementExportJob
description: Обновление свойств объекта deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aac5f773d14a22d1aea76319138e500028454ead
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52749047"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="055d5-103">Обновление deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="055d5-103">Update deviceManagementExportJob</span></span>

<span data-ttu-id="055d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="055d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="055d5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="055d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="055d5-106">Обновление свойств объекта [deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="055d5-106">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="055d5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="055d5-107">Prerequisites</span></span>
<span data-ttu-id="055d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="055d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="055d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="055d5-110">Permission type</span></span>|<span data-ttu-id="055d5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="055d5-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="055d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="055d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="055d5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="055d5-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="055d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="055d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="055d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="055d5-115">Not supported.</span></span>|
|<span data-ttu-id="055d5-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="055d5-116">Application</span></span>|<span data-ttu-id="055d5-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="055d5-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="055d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="055d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="055d5-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="055d5-119">Request headers</span></span>
|<span data-ttu-id="055d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="055d5-120">Header</span></span>|<span data-ttu-id="055d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="055d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="055d5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="055d5-122">Authorization</span></span>|<span data-ttu-id="055d5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="055d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="055d5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="055d5-124">Accept</span></span>|<span data-ttu-id="055d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="055d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="055d5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="055d5-126">Request body</span></span>
<span data-ttu-id="055d5-127">В теле запроса поставляем представление JSON для [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="055d5-127">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="055d5-128">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="055d5-128">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="055d5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="055d5-129">Property</span></span>|<span data-ttu-id="055d5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="055d5-130">Type</span></span>|<span data-ttu-id="055d5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="055d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="055d5-132">id</span><span class="sxs-lookup"><span data-stu-id="055d5-132">id</span></span>|<span data-ttu-id="055d5-133">String</span><span class="sxs-lookup"><span data-stu-id="055d5-133">String</span></span>|<span data-ttu-id="055d5-134">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="055d5-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="055d5-135">reportName</span><span class="sxs-lookup"><span data-stu-id="055d5-135">reportName</span></span>|<span data-ttu-id="055d5-136">String</span><span class="sxs-lookup"><span data-stu-id="055d5-136">String</span></span>|<span data-ttu-id="055d5-137">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="055d5-137">Name of the report</span></span>|
|<span data-ttu-id="055d5-138">filter</span><span class="sxs-lookup"><span data-stu-id="055d5-138">filter</span></span>|<span data-ttu-id="055d5-139">String</span><span class="sxs-lookup"><span data-stu-id="055d5-139">String</span></span>|<span data-ttu-id="055d5-140">Фильтры, применяемые в отчете</span><span class="sxs-lookup"><span data-stu-id="055d5-140">Filters applied on the report</span></span>|
|<span data-ttu-id="055d5-141">select</span><span class="sxs-lookup"><span data-stu-id="055d5-141">select</span></span>|<span data-ttu-id="055d5-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="055d5-142">String collection</span></span>|<span data-ttu-id="055d5-143">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="055d5-143">Columns selected from the report</span></span>|
|<span data-ttu-id="055d5-144">format</span><span class="sxs-lookup"><span data-stu-id="055d5-144">format</span></span>|[<span data-ttu-id="055d5-145">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="055d5-145">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="055d5-146">Формат экспортируемого отчета.</span><span class="sxs-lookup"><span data-stu-id="055d5-146">Format of the exported report.</span></span> <span data-ttu-id="055d5-147">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="055d5-147">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="055d5-148">snapshotId</span><span class="sxs-lookup"><span data-stu-id="055d5-148">snapshotId</span></span>|<span data-ttu-id="055d5-149">String</span><span class="sxs-lookup"><span data-stu-id="055d5-149">String</span></span>|<span data-ttu-id="055d5-150">Снимок — это идентифицируемый подмножество наборов данных, представленных в ReportName.</span><span class="sxs-lookup"><span data-stu-id="055d5-150">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="055d5-151">Здесь можно использовать id sessionId или CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="055d5-151">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="055d5-152">Если задана sessionId, фильтр, выберите и OrderBy применяются к данным, представленным sessionId.</span><span class="sxs-lookup"><span data-stu-id="055d5-152">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="055d5-153">Фильтр, выбор и OrderBy нельзя указать вместе с id CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="055d5-153">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="055d5-154">ЛокализацияТип</span><span class="sxs-lookup"><span data-stu-id="055d5-154">localizationType</span></span>|[<span data-ttu-id="055d5-155">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="055d5-155">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="055d5-156">Настройка локализации запрашиваемого задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="055d5-156">Configures how the requested export job is localized.</span></span> <span data-ttu-id="055d5-157">Возможные значения: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span><span class="sxs-lookup"><span data-stu-id="055d5-157">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="055d5-158">status</span><span class="sxs-lookup"><span data-stu-id="055d5-158">status</span></span>|[<span data-ttu-id="055d5-159">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="055d5-159">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="055d5-160">Состояние задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="055d5-160">Status of the export job.</span></span> <span data-ttu-id="055d5-161">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="055d5-161">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="055d5-162">url</span><span class="sxs-lookup"><span data-stu-id="055d5-162">url</span></span>|<span data-ttu-id="055d5-163">String</span><span class="sxs-lookup"><span data-stu-id="055d5-163">String</span></span>|<span data-ttu-id="055d5-164">Временное расположение экспортируемого отчета</span><span class="sxs-lookup"><span data-stu-id="055d5-164">Temporary location of the exported report</span></span>|
|<span data-ttu-id="055d5-165">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="055d5-165">requestDateTime</span></span>|<span data-ttu-id="055d5-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="055d5-166">DateTimeOffset</span></span>|<span data-ttu-id="055d5-167">Время запроса экспортируемой отчетности</span><span class="sxs-lookup"><span data-stu-id="055d5-167">Time that the exported report was requested</span></span>|
|<span data-ttu-id="055d5-168">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="055d5-168">expirationDateTime</span></span>|<span data-ttu-id="055d5-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="055d5-169">DateTimeOffset</span></span>|<span data-ttu-id="055d5-170">Время истечения срока действия экспортируемой отчетности</span><span class="sxs-lookup"><span data-stu-id="055d5-170">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="055d5-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="055d5-171">Response</span></span>
<span data-ttu-id="055d5-172">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="055d5-172">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="055d5-173">Пример</span><span class="sxs-lookup"><span data-stu-id="055d5-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="055d5-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="055d5-174">Request</span></span>
<span data-ttu-id="055d5-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="055d5-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
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
```

### <a name="response"></a><span data-ttu-id="055d5-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="055d5-176">Response</span></span>
<span data-ttu-id="055d5-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="055d5-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 504

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
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```




