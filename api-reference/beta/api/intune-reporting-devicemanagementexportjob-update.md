---
title: Обновление deviceManagementExportJob
description: Обновление свойств объекта deviceManagementExportJob.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ff338167a92062d57393228ff5861d04c6420e3b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442384"
---
# <a name="update-devicemanagementexportjob"></a><span data-ttu-id="05b30-103">Обновление deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="05b30-103">Update deviceManagementExportJob</span></span>

<span data-ttu-id="05b30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05b30-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05b30-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b30-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05b30-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05b30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05b30-107">Обновление свойств объекта [deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="05b30-107">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05b30-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="05b30-108">Prerequisites</span></span>
<span data-ttu-id="05b30-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05b30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05b30-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05b30-111">Permission type</span></span>|<span data-ttu-id="05b30-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="05b30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05b30-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05b30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05b30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b30-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="05b30-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05b30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05b30-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05b30-116">Not supported.</span></span>|
|<span data-ttu-id="05b30-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="05b30-117">Application</span></span>|<span data-ttu-id="05b30-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05b30-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="05b30-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05b30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## <a name="request-headers"></a><span data-ttu-id="05b30-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="05b30-120">Request headers</span></span>
|<span data-ttu-id="05b30-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05b30-121">Header</span></span>|<span data-ttu-id="05b30-122">Значение</span><span class="sxs-lookup"><span data-stu-id="05b30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05b30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05b30-123">Authorization</span></span>|<span data-ttu-id="05b30-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05b30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05b30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05b30-125">Accept</span></span>|<span data-ttu-id="05b30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05b30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05b30-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05b30-127">Request body</span></span>
<span data-ttu-id="05b30-128">В теле запроса поставляем представление JSON для [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="05b30-128">In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>

<span data-ttu-id="05b30-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)</span><span class="sxs-lookup"><span data-stu-id="05b30-129">The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>

|<span data-ttu-id="05b30-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="05b30-130">Property</span></span>|<span data-ttu-id="05b30-131">Тип</span><span class="sxs-lookup"><span data-stu-id="05b30-131">Type</span></span>|<span data-ttu-id="05b30-132">Описание</span><span class="sxs-lookup"><span data-stu-id="05b30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b30-133">id</span><span class="sxs-lookup"><span data-stu-id="05b30-133">id</span></span>|<span data-ttu-id="05b30-134">String</span><span class="sxs-lookup"><span data-stu-id="05b30-134">String</span></span>|<span data-ttu-id="05b30-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="05b30-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="05b30-136">reportName</span><span class="sxs-lookup"><span data-stu-id="05b30-136">reportName</span></span>|<span data-ttu-id="05b30-137">String</span><span class="sxs-lookup"><span data-stu-id="05b30-137">String</span></span>|<span data-ttu-id="05b30-138">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="05b30-138">Name of the report</span></span>|
|<span data-ttu-id="05b30-139">filter</span><span class="sxs-lookup"><span data-stu-id="05b30-139">filter</span></span>|<span data-ttu-id="05b30-140">String</span><span class="sxs-lookup"><span data-stu-id="05b30-140">String</span></span>|<span data-ttu-id="05b30-141">Фильтры, применяемые в отчете</span><span class="sxs-lookup"><span data-stu-id="05b30-141">Filters applied on the report</span></span>|
|<span data-ttu-id="05b30-142">select</span><span class="sxs-lookup"><span data-stu-id="05b30-142">select</span></span>|<span data-ttu-id="05b30-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="05b30-143">String collection</span></span>|<span data-ttu-id="05b30-144">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="05b30-144">Columns selected from the report</span></span>|
|<span data-ttu-id="05b30-145">format</span><span class="sxs-lookup"><span data-stu-id="05b30-145">format</span></span>|[<span data-ttu-id="05b30-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="05b30-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="05b30-147">Формат экспортируемого отчета.</span><span class="sxs-lookup"><span data-stu-id="05b30-147">Format of the exported report.</span></span> <span data-ttu-id="05b30-148">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="05b30-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="05b30-149">snapshotId</span><span class="sxs-lookup"><span data-stu-id="05b30-149">snapshotId</span></span>|<span data-ttu-id="05b30-150">String</span><span class="sxs-lookup"><span data-stu-id="05b30-150">String</span></span>|<span data-ttu-id="05b30-151">Снимок — это идентифицируемый подмножество наборов данных, представленных в ReportName.</span><span class="sxs-lookup"><span data-stu-id="05b30-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="05b30-152">Здесь можно использовать id sessionId или CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05b30-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="05b30-153">Если задана sessionId, фильтр, выберите и OrderBy применяются к данным, представленным sessionId.</span><span class="sxs-lookup"><span data-stu-id="05b30-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="05b30-154">Фильтр, выбор и OrderBy нельзя указать вместе с id CachedReportConfiguration.</span><span class="sxs-lookup"><span data-stu-id="05b30-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="05b30-155">ЛокализацияТип</span><span class="sxs-lookup"><span data-stu-id="05b30-155">localizationType</span></span>|[<span data-ttu-id="05b30-156">deviceManagementExportJobLocalizationType</span><span class="sxs-lookup"><span data-stu-id="05b30-156">deviceManagementExportJobLocalizationType</span></span>](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|<span data-ttu-id="05b30-157">Настройка локализации запрашиваемого задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="05b30-157">Configures how the requested export job is localized.</span></span> <span data-ttu-id="05b30-158">Возможные значения: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span><span class="sxs-lookup"><span data-stu-id="05b30-158">Possible values are: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.</span></span>|
|<span data-ttu-id="05b30-159">status</span><span class="sxs-lookup"><span data-stu-id="05b30-159">status</span></span>|[<span data-ttu-id="05b30-160">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="05b30-160">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="05b30-161">Состояние задания экспорта.</span><span class="sxs-lookup"><span data-stu-id="05b30-161">Status of the export job.</span></span> <span data-ttu-id="05b30-162">Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="05b30-162">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="05b30-163">url</span><span class="sxs-lookup"><span data-stu-id="05b30-163">url</span></span>|<span data-ttu-id="05b30-164">String</span><span class="sxs-lookup"><span data-stu-id="05b30-164">String</span></span>|<span data-ttu-id="05b30-165">Временное расположение экспортируемого отчета</span><span class="sxs-lookup"><span data-stu-id="05b30-165">Temporary location of the exported report</span></span>|
|<span data-ttu-id="05b30-166">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="05b30-166">requestDateTime</span></span>|<span data-ttu-id="05b30-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b30-167">DateTimeOffset</span></span>|<span data-ttu-id="05b30-168">Время запроса экспортируемой отчетности</span><span class="sxs-lookup"><span data-stu-id="05b30-168">Time that the exported report was requested</span></span>|
|<span data-ttu-id="05b30-169">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="05b30-169">expirationDateTime</span></span>|<span data-ttu-id="05b30-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05b30-170">DateTimeOffset</span></span>|<span data-ttu-id="05b30-171">Время истечения срока действия экспортируемой отчетности</span><span class="sxs-lookup"><span data-stu-id="05b30-171">Time that the exported report expires</span></span>|



## <a name="response"></a><span data-ttu-id="05b30-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b30-172">Response</span></span>
<span data-ttu-id="05b30-173">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="05b30-173">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05b30-174">Пример</span><span class="sxs-lookup"><span data-stu-id="05b30-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="05b30-175">Запрос</span><span class="sxs-lookup"><span data-stu-id="05b30-175">Request</span></span>
<span data-ttu-id="05b30-176">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05b30-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
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

### <a name="response"></a><span data-ttu-id="05b30-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="05b30-177">Response</span></span>
<span data-ttu-id="05b30-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05b30-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




