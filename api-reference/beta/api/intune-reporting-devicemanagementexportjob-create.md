---
title: Создание deviceManagementExportJob
description: Создание нового объекта deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a126023796b92d8158d7875913efff9be6cf9695
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158460"
---
# <a name="create-devicemanagementexportjob"></a><span data-ttu-id="68414-103">Создание deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="68414-103">Create deviceManagementExportJob</span></span>

<span data-ttu-id="68414-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68414-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68414-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68414-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68414-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68414-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68414-107">Создание нового [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="68414-107">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68414-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68414-108">Prerequisites</span></span>
<span data-ttu-id="68414-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68414-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68414-111">Permission type</span></span>|<span data-ttu-id="68414-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68414-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68414-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68414-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68414-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68414-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="68414-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68414-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68414-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68414-116">Not supported.</span></span>|
|<span data-ttu-id="68414-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="68414-117">Application</span></span>|<span data-ttu-id="68414-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68414-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="68414-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68414-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a><span data-ttu-id="68414-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="68414-120">Request headers</span></span>
|<span data-ttu-id="68414-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68414-121">Header</span></span>|<span data-ttu-id="68414-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68414-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68414-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="68414-123">Authorization</span></span>|<span data-ttu-id="68414-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68414-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68414-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68414-125">Accept</span></span>|<span data-ttu-id="68414-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68414-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68414-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68414-127">Request body</span></span>
<span data-ttu-id="68414-128">В теле запроса поставляем представление JSON для объекта deviceManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="68414-128">In the request body, supply a JSON representation for the deviceManagementExportJob object.</span></span>

<span data-ttu-id="68414-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementExportJob.</span><span class="sxs-lookup"><span data-stu-id="68414-129">The following table shows the properties that are required when you create the deviceManagementExportJob.</span></span>

|<span data-ttu-id="68414-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="68414-130">Property</span></span>|<span data-ttu-id="68414-131">Тип</span><span class="sxs-lookup"><span data-stu-id="68414-131">Type</span></span>|<span data-ttu-id="68414-132">Описание</span><span class="sxs-lookup"><span data-stu-id="68414-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68414-133">id</span><span class="sxs-lookup"><span data-stu-id="68414-133">id</span></span>|<span data-ttu-id="68414-134">Строка</span><span class="sxs-lookup"><span data-stu-id="68414-134">String</span></span>|<span data-ttu-id="68414-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="68414-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="68414-136">reportName</span><span class="sxs-lookup"><span data-stu-id="68414-136">reportName</span></span>|<span data-ttu-id="68414-137">Строка</span><span class="sxs-lookup"><span data-stu-id="68414-137">String</span></span>|<span data-ttu-id="68414-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="68414-138">Name of the report</span></span>|
|<span data-ttu-id="68414-139">filter</span><span class="sxs-lookup"><span data-stu-id="68414-139">filter</span></span>|<span data-ttu-id="68414-140">Строка</span><span class="sxs-lookup"><span data-stu-id="68414-140">String</span></span>|<span data-ttu-id="68414-141">Фильтры, применяемые в отчете</span><span class="sxs-lookup"><span data-stu-id="68414-141">Filters applied on the report</span></span>|
|<span data-ttu-id="68414-142">select</span><span class="sxs-lookup"><span data-stu-id="68414-142">select</span></span>|<span data-ttu-id="68414-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="68414-143">String collection</span></span>|<span data-ttu-id="68414-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="68414-144">Columns selected from the report</span></span>|
|<span data-ttu-id="68414-145">format</span><span class="sxs-lookup"><span data-stu-id="68414-145">format</span></span>|[<span data-ttu-id="68414-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="68414-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="68414-147">Формат экспортируемого отчета.</span><span class="sxs-lookup"><span data-stu-id="68414-147">Format of the exported report.</span></span> <span data-ttu-id="68414-148">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="68414-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="68414-149">snapshotId</span><span class="sxs-lookup"><span data-stu-id="68414-149">snapshotId</span></span>|<span data-ttu-id="68414-150">Строка</span><span class="sxs-lookup"><span data-stu-id="68414-150">String</span></span>|<span data-ttu-id="68414-151">Снимок — это идентифицируемый подмножество наборов данных, представленных в ReportName.</span><span class="sxs-lookup"><span data-stu-id="68414-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="68414-152">Здесь можно использовать id sessionId или CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68414-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="68414-153">Если задана sessionId, фильтр, выберите и OrderBy применяются к данным, представленным sessionId.</span><span class="sxs-lookup"><span data-stu-id="68414-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="68414-154">Фильтр, выбор и OrderBy нельзя указать вместе с id CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="68414-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="68414-155">ЛокализацияТип</span><span class="sxs-lookup"><span data-stu-id="68414-155">localizationType</span></span>|[<span data-ttu-id="68414-156">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="68414-156">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="68414-157">Настройка локализации запрашиваемого задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="68414-157">Configures how the requested export job is localized.</span></span> <span data-ttu-id="68414-158">Возможные значения: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span><span class="sxs-lookup"><span data-stu-id="68414-158">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="68414-159">status</span><span class="sxs-lookup"><span data-stu-id="68414-159">status</span></span>|[<span data-ttu-id="68414-160">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="68414-160">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="68414-161">Состояние задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="68414-161">Status of the export job.</span></span> <span data-ttu-id="68414-162">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="68414-162">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="68414-163">url</span><span class="sxs-lookup"><span data-stu-id="68414-163">url</span></span>|<span data-ttu-id="68414-164">String</span><span class="sxs-lookup"><span data-stu-id="68414-164">String</span></span>|<span data-ttu-id="68414-165">Временное расположение экспортируемого отчета</span><span class="sxs-lookup"><span data-stu-id="68414-165">Temporary location of the exported report</span></span>|
|<span data-ttu-id="68414-166">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="68414-166">requestDateTime</span></span>|<span data-ttu-id="68414-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68414-167">DateTimeOffset</span></span>|<span data-ttu-id="68414-168">Время запроса экспортируемой отчетности</span><span class="sxs-lookup"><span data-stu-id="68414-168">Time that the exported report was requested</span></span>|
|<span data-ttu-id="68414-169">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="68414-169">expirationDateTime</span></span>|<span data-ttu-id="68414-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68414-170">DateTimeOffset</span></span>|<span data-ttu-id="68414-171">Время истечения срока действия экспортируемой отчетности</span><span class="sxs-lookup"><span data-stu-id="68414-171">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="68414-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="68414-172">Response</span></span>
<span data-ttu-id="68414-173">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="68414-173">If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68414-174">Пример</span><span class="sxs-lookup"><span data-stu-id="68414-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="68414-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="68414-175">Request</span></span>
<span data-ttu-id="68414-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68414-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
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

### <a name="response"></a><span data-ttu-id="68414-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="68414-177">Response</span></span>
<span data-ttu-id="68414-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68414-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




