---
title: Обновление deviceManagementReportSchedule
description: Обновление свойств объекта deviceManagementReportSchedule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2e1466e9a24ba3cd4021ed7d8aa59897af017354
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134377"
---
# <a name="update-devicemanagementreportschedule"></a><span data-ttu-id="0a665-103">Обновление deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="0a665-103">Update deviceManagementReportSchedule</span></span>

<span data-ttu-id="0a665-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a665-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a665-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a665-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a665-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a665-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a665-107">Обновление свойств объекта [deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)</span><span class="sxs-lookup"><span data-stu-id="0a665-107">Update the properties of a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a665-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0a665-108">Prerequisites</span></span>
<span data-ttu-id="0a665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a665-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a665-111">Permission type</span></span>|<span data-ttu-id="0a665-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a665-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a665-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a665-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0a665-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a665-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0a665-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a665-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a665-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a665-116">Not supported.</span></span>|
|<span data-ttu-id="0a665-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a665-117">Application</span></span>|<span data-ttu-id="0a665-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a665-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a665-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a665-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="request-headers"></a><span data-ttu-id="0a665-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0a665-120">Request headers</span></span>
|<span data-ttu-id="0a665-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a665-121">Header</span></span>|<span data-ttu-id="0a665-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0a665-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a665-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a665-123">Authorization</span></span>|<span data-ttu-id="0a665-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a665-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a665-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0a665-125">Accept</span></span>|<span data-ttu-id="0a665-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0a665-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a665-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a665-127">Request body</span></span>
<span data-ttu-id="0a665-128">В теле запроса поставляем представление JSON для [объекта deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)</span><span class="sxs-lookup"><span data-stu-id="0a665-128">In the request body, supply a JSON representation for the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

<span data-ttu-id="0a665-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)</span><span class="sxs-lookup"><span data-stu-id="0a665-129">The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).</span></span>

|<span data-ttu-id="0a665-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a665-130">Property</span></span>|<span data-ttu-id="0a665-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0a665-131">Type</span></span>|<span data-ttu-id="0a665-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0a665-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a665-133">id</span><span class="sxs-lookup"><span data-stu-id="0a665-133">id</span></span>|<span data-ttu-id="0a665-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0a665-134">String</span></span>|<span data-ttu-id="0a665-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="0a665-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="0a665-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="0a665-136">reportScheduleName</span></span>|<span data-ttu-id="0a665-137">Строка</span><span class="sxs-lookup"><span data-stu-id="0a665-137">String</span></span>|<span data-ttu-id="0a665-138">Имя расписания</span><span class="sxs-lookup"><span data-stu-id="0a665-138">Name of the schedule</span></span>|
|<span data-ttu-id="0a665-139">subject</span><span class="sxs-lookup"><span data-stu-id="0a665-139">subject</span></span>|<span data-ttu-id="0a665-140">String</span><span class="sxs-lookup"><span data-stu-id="0a665-140">String</span></span>|<span data-ttu-id="0a665-141">Тема запланированных отчетов, которые будут доставлены</span><span class="sxs-lookup"><span data-stu-id="0a665-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="0a665-142">электронные письма</span><span class="sxs-lookup"><span data-stu-id="0a665-142">emails</span></span>|<span data-ttu-id="0a665-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a665-143">String collection</span></span>|<span data-ttu-id="0a665-144">Сообщения электронной почты, на которые доставляются запланированные отчеты</span><span class="sxs-lookup"><span data-stu-id="0a665-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="0a665-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="0a665-145">recurrence</span></span>|[<span data-ttu-id="0a665-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="0a665-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="0a665-147">Частота доставки отчетов по расписанию.</span><span class="sxs-lookup"><span data-stu-id="0a665-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="0a665-148">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="0a665-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="0a665-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0a665-149">startDateTime</span></span>|<span data-ttu-id="0a665-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a665-150">DateTimeOffset</span></span>|<span data-ttu-id="0a665-151">Время начала доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="0a665-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="0a665-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="0a665-152">endDateTime</span></span>|<span data-ttu-id="0a665-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a665-153">DateTimeOffset</span></span>|<span data-ttu-id="0a665-154">Время окончания доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="0a665-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="0a665-155">userId</span><span class="sxs-lookup"><span data-stu-id="0a665-155">userId</span></span>|<span data-ttu-id="0a665-156">String</span><span class="sxs-lookup"><span data-stu-id="0a665-156">String</span></span>|<span data-ttu-id="0a665-157">Id пользователя, создавшего отчет</span><span class="sxs-lookup"><span data-stu-id="0a665-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="0a665-158">reportName</span><span class="sxs-lookup"><span data-stu-id="0a665-158">reportName</span></span>|<span data-ttu-id="0a665-159">Строка</span><span class="sxs-lookup"><span data-stu-id="0a665-159">String</span></span>|<span data-ttu-id="0a665-160">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="0a665-160">Name of the report</span></span>|
|<span data-ttu-id="0a665-161">filter</span><span class="sxs-lookup"><span data-stu-id="0a665-161">filter</span></span>|<span data-ttu-id="0a665-162">Строка</span><span class="sxs-lookup"><span data-stu-id="0a665-162">String</span></span>|<span data-ttu-id="0a665-163">Фильтры, применяемые в отчете</span><span class="sxs-lookup"><span data-stu-id="0a665-163">Filters applied on the report</span></span>|
|<span data-ttu-id="0a665-164">select</span><span class="sxs-lookup"><span data-stu-id="0a665-164">select</span></span>|<span data-ttu-id="0a665-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a665-165">String collection</span></span>|<span data-ttu-id="0a665-166">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="0a665-166">Columns selected from the report</span></span>|
|<span data-ttu-id="0a665-167">orderBy</span><span class="sxs-lookup"><span data-stu-id="0a665-167">orderBy</span></span>|<span data-ttu-id="0a665-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a665-168">String collection</span></span>|<span data-ttu-id="0a665-169">Порядок столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="0a665-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="0a665-170">format</span><span class="sxs-lookup"><span data-stu-id="0a665-170">format</span></span>|[<span data-ttu-id="0a665-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="0a665-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="0a665-172">Формат запланированного отчета.</span><span class="sxs-lookup"><span data-stu-id="0a665-172">Format of the scheduled report.</span></span> <span data-ttu-id="0a665-173">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="0a665-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="0a665-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a665-174">Response</span></span>
<span data-ttu-id="0a665-175">В случае успешного выполнения этот метод возвращает код ответа и обновленный `200 OK` [объект deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0a665-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a665-176">Пример</span><span class="sxs-lookup"><span data-stu-id="0a665-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a665-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a665-177">Request</span></span>
<span data-ttu-id="0a665-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a665-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
Content-type: application/json
Content-length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```

### <a name="response"></a><span data-ttu-id="0a665-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a665-179">Response</span></span>
<span data-ttu-id="0a665-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0a665-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 588

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "00bb9785-9785-00bb-8597-bb008597bb00",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "daily",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "pdf"
}
```




