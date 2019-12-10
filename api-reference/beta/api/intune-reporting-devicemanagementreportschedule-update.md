---
title: Обновление Девицеманажементрепортсчедуле
description: Обновление свойств объекта Девицеманажементрепортсчедуле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7506d298f094e8528c24813c9df86720866b9090
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940238"
---
# <a name="update-devicemanagementreportschedule"></a><span data-ttu-id="92465-103">Обновление Девицеманажементрепортсчедуле</span><span class="sxs-lookup"><span data-stu-id="92465-103">Update deviceManagementReportSchedule</span></span>

> <span data-ttu-id="92465-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92465-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92465-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92465-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92465-106">Обновление свойств объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="92465-106">Update the properties of a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92465-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="92465-107">Prerequisites</span></span>
<span data-ttu-id="92465-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92465-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92465-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="92465-110">Permission type</span></span>|<span data-ttu-id="92465-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="92465-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92465-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="92465-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92465-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="92465-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="92465-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="92465-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92465-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92465-115">Not supported.</span></span>|
|<span data-ttu-id="92465-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="92465-116">Application</span></span>|<span data-ttu-id="92465-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="92465-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92465-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="92465-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="request-headers"></a><span data-ttu-id="92465-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="92465-119">Request headers</span></span>
|<span data-ttu-id="92465-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="92465-120">Header</span></span>|<span data-ttu-id="92465-121">Значение</span><span class="sxs-lookup"><span data-stu-id="92465-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92465-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="92465-122">Authorization</span></span>|<span data-ttu-id="92465-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="92465-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92465-124">Accept</span><span class="sxs-lookup"><span data-stu-id="92465-124">Accept</span></span>|<span data-ttu-id="92465-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92465-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92465-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="92465-126">Request body</span></span>
<span data-ttu-id="92465-127">В тексте запроса добавьте представление объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92465-127">In the request body, supply a JSON representation for the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

<span data-ttu-id="92465-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md).</span><span class="sxs-lookup"><span data-stu-id="92465-128">The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).</span></span>

|<span data-ttu-id="92465-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="92465-129">Property</span></span>|<span data-ttu-id="92465-130">Тип</span><span class="sxs-lookup"><span data-stu-id="92465-130">Type</span></span>|<span data-ttu-id="92465-131">Описание</span><span class="sxs-lookup"><span data-stu-id="92465-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92465-132">id</span><span class="sxs-lookup"><span data-stu-id="92465-132">id</span></span>|<span data-ttu-id="92465-133">Строка</span><span class="sxs-lookup"><span data-stu-id="92465-133">String</span></span>|<span data-ttu-id="92465-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="92465-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="92465-135">репортсчедуленаме</span><span class="sxs-lookup"><span data-stu-id="92465-135">reportScheduleName</span></span>|<span data-ttu-id="92465-136">Строка</span><span class="sxs-lookup"><span data-stu-id="92465-136">String</span></span>|<span data-ttu-id="92465-137">Имя расписания</span><span class="sxs-lookup"><span data-stu-id="92465-137">Name of the schedule</span></span>|
|<span data-ttu-id="92465-138">subject</span><span class="sxs-lookup"><span data-stu-id="92465-138">subject</span></span>|<span data-ttu-id="92465-139">String</span><span class="sxs-lookup"><span data-stu-id="92465-139">String</span></span>|<span data-ttu-id="92465-140">Тема запланированных отчетов, которые доставляются</span><span class="sxs-lookup"><span data-stu-id="92465-140">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="92465-141">письма</span><span class="sxs-lookup"><span data-stu-id="92465-141">emails</span></span>|<span data-ttu-id="92465-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="92465-142">String collection</span></span>|<span data-ttu-id="92465-143">Сообщения электронной почты, на которые доставляются запланированные отчеты</span><span class="sxs-lookup"><span data-stu-id="92465-143">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="92465-144">recurrence</span><span class="sxs-lookup"><span data-stu-id="92465-144">recurrence</span></span>|[<span data-ttu-id="92465-145">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="92465-145">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="92465-146">Периодичность запланированной доставки отчета.</span><span class="sxs-lookup"><span data-stu-id="92465-146">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="92465-147">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="92465-147">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="92465-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="92465-148">startDateTime</span></span>|<span data-ttu-id="92465-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92465-149">DateTimeOffset</span></span>|<span data-ttu-id="92465-150">Время, когда начинается доставка запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="92465-150">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="92465-151">endDateTime</span><span class="sxs-lookup"><span data-stu-id="92465-151">endDateTime</span></span>|<span data-ttu-id="92465-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92465-152">DateTimeOffset</span></span>|<span data-ttu-id="92465-153">Время окончания доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="92465-153">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="92465-154">userId</span><span class="sxs-lookup"><span data-stu-id="92465-154">userId</span></span>|<span data-ttu-id="92465-155">String</span><span class="sxs-lookup"><span data-stu-id="92465-155">String</span></span>|<span data-ttu-id="92465-156">Идентификатор пользователя, создавшего отчет</span><span class="sxs-lookup"><span data-stu-id="92465-156">The Id of the User who created the report</span></span>|
|<span data-ttu-id="92465-157">репортнаме</span><span class="sxs-lookup"><span data-stu-id="92465-157">reportName</span></span>|<span data-ttu-id="92465-158">Строка</span><span class="sxs-lookup"><span data-stu-id="92465-158">String</span></span>|<span data-ttu-id="92465-159">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="92465-159">Name of the report</span></span>|
|<span data-ttu-id="92465-160">filter</span><span class="sxs-lookup"><span data-stu-id="92465-160">filter</span></span>|<span data-ttu-id="92465-161">Строка</span><span class="sxs-lookup"><span data-stu-id="92465-161">String</span></span>|<span data-ttu-id="92465-162">Фильтры, примененные к отчету</span><span class="sxs-lookup"><span data-stu-id="92465-162">Filters applied on the report</span></span>|
|<span data-ttu-id="92465-163">select</span><span class="sxs-lookup"><span data-stu-id="92465-163">select</span></span>|<span data-ttu-id="92465-164">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="92465-164">String collection</span></span>|<span data-ttu-id="92465-165">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="92465-165">Columns selected from the report</span></span>|
|<span data-ttu-id="92465-166">orderBy</span><span class="sxs-lookup"><span data-stu-id="92465-166">orderBy</span></span>|<span data-ttu-id="92465-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="92465-167">String collection</span></span>|<span data-ttu-id="92465-168">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="92465-168">Ordering of columns in the report</span></span>|
|<span data-ttu-id="92465-169">format</span><span class="sxs-lookup"><span data-stu-id="92465-169">format</span></span>|[<span data-ttu-id="92465-170">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="92465-170">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="92465-171">Формат запланированного отчета.</span><span class="sxs-lookup"><span data-stu-id="92465-171">Format of the scheduled report.</span></span> <span data-ttu-id="92465-172">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="92465-172">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="92465-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="92465-173">Response</span></span>
<span data-ttu-id="92465-174">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="92465-174">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92465-175">Пример</span><span class="sxs-lookup"><span data-stu-id="92465-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="92465-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="92465-176">Request</span></span>
<span data-ttu-id="92465-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="92465-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92465-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="92465-178">Response</span></span>
<span data-ttu-id="92465-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="92465-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





