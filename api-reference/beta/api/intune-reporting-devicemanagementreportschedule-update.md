---
title: Обновление Девицеманажементрепортсчедуле
description: Обновление свойств объекта Девицеманажементрепортсчедуле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7fbc512c97f96b1aecf88533628997a871faa131
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698073"
---
# <a name="update-devicemanagementreportschedule"></a><span data-ttu-id="38d6d-103">Обновление Девицеманажементрепортсчедуле</span><span class="sxs-lookup"><span data-stu-id="38d6d-103">Update deviceManagementReportSchedule</span></span>

<span data-ttu-id="38d6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38d6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38d6d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38d6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38d6d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38d6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38d6d-107">Обновление свойств объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="38d6d-107">Update the properties of a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38d6d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="38d6d-108">Prerequisites</span></span>
<span data-ttu-id="38d6d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38d6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38d6d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38d6d-111">Permission type</span></span>|<span data-ttu-id="38d6d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38d6d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38d6d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38d6d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38d6d-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="38d6d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="38d6d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38d6d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38d6d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38d6d-116">Not supported.</span></span>|
|<span data-ttu-id="38d6d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38d6d-117">Application</span></span>|<span data-ttu-id="38d6d-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="38d6d-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38d6d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38d6d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="request-headers"></a><span data-ttu-id="38d6d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38d6d-120">Request headers</span></span>
|<span data-ttu-id="38d6d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38d6d-121">Header</span></span>|<span data-ttu-id="38d6d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="38d6d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38d6d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38d6d-123">Authorization</span></span>|<span data-ttu-id="38d6d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38d6d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38d6d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38d6d-125">Accept</span></span>|<span data-ttu-id="38d6d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38d6d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38d6d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38d6d-127">Request body</span></span>
<span data-ttu-id="38d6d-128">В тексте запроса добавьте представление объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38d6d-128">In the request body, supply a JSON representation for the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

<span data-ttu-id="38d6d-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md).</span><span class="sxs-lookup"><span data-stu-id="38d6d-129">The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md).</span></span>

|<span data-ttu-id="38d6d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="38d6d-130">Property</span></span>|<span data-ttu-id="38d6d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="38d6d-131">Type</span></span>|<span data-ttu-id="38d6d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="38d6d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38d6d-133">id</span><span class="sxs-lookup"><span data-stu-id="38d6d-133">id</span></span>|<span data-ttu-id="38d6d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="38d6d-134">String</span></span>|<span data-ttu-id="38d6d-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="38d6d-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="38d6d-136">репортсчедуленаме</span><span class="sxs-lookup"><span data-stu-id="38d6d-136">reportScheduleName</span></span>|<span data-ttu-id="38d6d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="38d6d-137">String</span></span>|<span data-ttu-id="38d6d-138">Имя расписания</span><span class="sxs-lookup"><span data-stu-id="38d6d-138">Name of the schedule</span></span>|
|<span data-ttu-id="38d6d-139">subject</span><span class="sxs-lookup"><span data-stu-id="38d6d-139">subject</span></span>|<span data-ttu-id="38d6d-140">String</span><span class="sxs-lookup"><span data-stu-id="38d6d-140">String</span></span>|<span data-ttu-id="38d6d-141">Тема запланированных отчетов, которые доставляются</span><span class="sxs-lookup"><span data-stu-id="38d6d-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="38d6d-142">письма</span><span class="sxs-lookup"><span data-stu-id="38d6d-142">emails</span></span>|<span data-ttu-id="38d6d-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="38d6d-143">String collection</span></span>|<span data-ttu-id="38d6d-144">Сообщения электронной почты, на которые доставляются запланированные отчеты</span><span class="sxs-lookup"><span data-stu-id="38d6d-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="38d6d-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="38d6d-145">recurrence</span></span>|[<span data-ttu-id="38d6d-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="38d6d-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="38d6d-147">Периодичность запланированной доставки отчета.</span><span class="sxs-lookup"><span data-stu-id="38d6d-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="38d6d-148">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="38d6d-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="38d6d-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="38d6d-149">startDateTime</span></span>|<span data-ttu-id="38d6d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38d6d-150">DateTimeOffset</span></span>|<span data-ttu-id="38d6d-151">Время, когда начинается доставка запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="38d6d-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="38d6d-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="38d6d-152">endDateTime</span></span>|<span data-ttu-id="38d6d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38d6d-153">DateTimeOffset</span></span>|<span data-ttu-id="38d6d-154">Время окончания доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="38d6d-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="38d6d-155">userId</span><span class="sxs-lookup"><span data-stu-id="38d6d-155">userId</span></span>|<span data-ttu-id="38d6d-156">String</span><span class="sxs-lookup"><span data-stu-id="38d6d-156">String</span></span>|<span data-ttu-id="38d6d-157">Идентификатор пользователя, создавшего отчет</span><span class="sxs-lookup"><span data-stu-id="38d6d-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="38d6d-158">репортнаме</span><span class="sxs-lookup"><span data-stu-id="38d6d-158">reportName</span></span>|<span data-ttu-id="38d6d-159">Строка</span><span class="sxs-lookup"><span data-stu-id="38d6d-159">String</span></span>|<span data-ttu-id="38d6d-160">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="38d6d-160">Name of the report</span></span>|
|<span data-ttu-id="38d6d-161">filter</span><span class="sxs-lookup"><span data-stu-id="38d6d-161">filter</span></span>|<span data-ttu-id="38d6d-162">Строка</span><span class="sxs-lookup"><span data-stu-id="38d6d-162">String</span></span>|<span data-ttu-id="38d6d-163">Фильтры, примененные к отчету</span><span class="sxs-lookup"><span data-stu-id="38d6d-163">Filters applied on the report</span></span>|
|<span data-ttu-id="38d6d-164">select</span><span class="sxs-lookup"><span data-stu-id="38d6d-164">select</span></span>|<span data-ttu-id="38d6d-165">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="38d6d-165">String collection</span></span>|<span data-ttu-id="38d6d-166">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="38d6d-166">Columns selected from the report</span></span>|
|<span data-ttu-id="38d6d-167">orderBy</span><span class="sxs-lookup"><span data-stu-id="38d6d-167">orderBy</span></span>|<span data-ttu-id="38d6d-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="38d6d-168">String collection</span></span>|<span data-ttu-id="38d6d-169">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="38d6d-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="38d6d-170">format</span><span class="sxs-lookup"><span data-stu-id="38d6d-170">format</span></span>|[<span data-ttu-id="38d6d-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="38d6d-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="38d6d-172">Формат запланированного отчета.</span><span class="sxs-lookup"><span data-stu-id="38d6d-172">Format of the scheduled report.</span></span> <span data-ttu-id="38d6d-173">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="38d6d-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="38d6d-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="38d6d-174">Response</span></span>
<span data-ttu-id="38d6d-175">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38d6d-175">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38d6d-176">Пример</span><span class="sxs-lookup"><span data-stu-id="38d6d-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="38d6d-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="38d6d-177">Request</span></span>
<span data-ttu-id="38d6d-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38d6d-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38d6d-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="38d6d-179">Response</span></span>
<span data-ttu-id="38d6d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38d6d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





