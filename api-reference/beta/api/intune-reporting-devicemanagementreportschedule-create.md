---
title: Создание deviceManagementReportSchedule
description: Создание нового объекта deviceManagementReportSchedule.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a9e29979c0999d05592adaad8e2f19a332a57a8a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134391"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="f030b-103">Создание deviceManagementReportSchedule</span><span class="sxs-lookup"><span data-stu-id="f030b-103">Create deviceManagementReportSchedule</span></span>

<span data-ttu-id="f030b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f030b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f030b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f030b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f030b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f030b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f030b-107">Создание нового [объекта deviceManagementReportSchedule.](../resources/intune-reporting-devicemanagementreportschedule.md)</span><span class="sxs-lookup"><span data-stu-id="f030b-107">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f030b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f030b-108">Prerequisites</span></span>
<span data-ttu-id="f030b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f030b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f030b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f030b-111">Permission type</span></span>|<span data-ttu-id="f030b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f030b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f030b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f030b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f030b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f030b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f030b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f030b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f030b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f030b-116">Not supported.</span></span>|
|<span data-ttu-id="f030b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f030b-117">Application</span></span>|<span data-ttu-id="f030b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f030b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f030b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f030b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="f030b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f030b-120">Request headers</span></span>
|<span data-ttu-id="f030b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f030b-121">Header</span></span>|<span data-ttu-id="f030b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f030b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f030b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f030b-123">Authorization</span></span>|<span data-ttu-id="f030b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f030b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f030b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f030b-125">Accept</span></span>|<span data-ttu-id="f030b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f030b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f030b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f030b-127">Request body</span></span>
<span data-ttu-id="f030b-128">В теле запроса поставляем представление JSON для объекта deviceManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="f030b-128">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="f030b-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementReportSchedule.</span><span class="sxs-lookup"><span data-stu-id="f030b-129">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="f030b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f030b-130">Property</span></span>|<span data-ttu-id="f030b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f030b-131">Type</span></span>|<span data-ttu-id="f030b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f030b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f030b-133">id</span><span class="sxs-lookup"><span data-stu-id="f030b-133">id</span></span>|<span data-ttu-id="f030b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f030b-134">String</span></span>|<span data-ttu-id="f030b-135">Уникальный идентификатор для этого объекта</span><span class="sxs-lookup"><span data-stu-id="f030b-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="f030b-136">reportScheduleName</span><span class="sxs-lookup"><span data-stu-id="f030b-136">reportScheduleName</span></span>|<span data-ttu-id="f030b-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f030b-137">String</span></span>|<span data-ttu-id="f030b-138">Имя расписания</span><span class="sxs-lookup"><span data-stu-id="f030b-138">Name of the schedule</span></span>|
|<span data-ttu-id="f030b-139">subject</span><span class="sxs-lookup"><span data-stu-id="f030b-139">subject</span></span>|<span data-ttu-id="f030b-140">String</span><span class="sxs-lookup"><span data-stu-id="f030b-140">String</span></span>|<span data-ttu-id="f030b-141">Тема запланированных отчетов, которые будут доставлены</span><span class="sxs-lookup"><span data-stu-id="f030b-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="f030b-142">электронные письма</span><span class="sxs-lookup"><span data-stu-id="f030b-142">emails</span></span>|<span data-ttu-id="f030b-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f030b-143">String collection</span></span>|<span data-ttu-id="f030b-144">Сообщения электронной почты, на которые доставляются запланированные отчеты</span><span class="sxs-lookup"><span data-stu-id="f030b-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="f030b-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="f030b-145">recurrence</span></span>|[<span data-ttu-id="f030b-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="f030b-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="f030b-147">Частота доставки отчетов по расписанию.</span><span class="sxs-lookup"><span data-stu-id="f030b-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="f030b-148">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="f030b-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="f030b-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f030b-149">startDateTime</span></span>|<span data-ttu-id="f030b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f030b-150">DateTimeOffset</span></span>|<span data-ttu-id="f030b-151">Время начала доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="f030b-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="f030b-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f030b-152">endDateTime</span></span>|<span data-ttu-id="f030b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f030b-153">DateTimeOffset</span></span>|<span data-ttu-id="f030b-154">Время окончания доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="f030b-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="f030b-155">userId</span><span class="sxs-lookup"><span data-stu-id="f030b-155">userId</span></span>|<span data-ttu-id="f030b-156">String</span><span class="sxs-lookup"><span data-stu-id="f030b-156">String</span></span>|<span data-ttu-id="f030b-157">Id пользователя, создавшего отчет</span><span class="sxs-lookup"><span data-stu-id="f030b-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="f030b-158">reportName</span><span class="sxs-lookup"><span data-stu-id="f030b-158">reportName</span></span>|<span data-ttu-id="f030b-159">Строка</span><span class="sxs-lookup"><span data-stu-id="f030b-159">String</span></span>|<span data-ttu-id="f030b-160">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="f030b-160">Name of the report</span></span>|
|<span data-ttu-id="f030b-161">filter</span><span class="sxs-lookup"><span data-stu-id="f030b-161">filter</span></span>|<span data-ttu-id="f030b-162">Строка</span><span class="sxs-lookup"><span data-stu-id="f030b-162">String</span></span>|<span data-ttu-id="f030b-163">Фильтры, применяемые в отчете</span><span class="sxs-lookup"><span data-stu-id="f030b-163">Filters applied on the report</span></span>|
|<span data-ttu-id="f030b-164">select</span><span class="sxs-lookup"><span data-stu-id="f030b-164">select</span></span>|<span data-ttu-id="f030b-165">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f030b-165">String collection</span></span>|<span data-ttu-id="f030b-166">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="f030b-166">Columns selected from the report</span></span>|
|<span data-ttu-id="f030b-167">orderBy</span><span class="sxs-lookup"><span data-stu-id="f030b-167">orderBy</span></span>|<span data-ttu-id="f030b-168">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="f030b-168">String collection</span></span>|<span data-ttu-id="f030b-169">Порядок столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="f030b-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="f030b-170">format</span><span class="sxs-lookup"><span data-stu-id="f030b-170">format</span></span>|[<span data-ttu-id="f030b-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="f030b-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="f030b-172">Формат запланированного отчета.</span><span class="sxs-lookup"><span data-stu-id="f030b-172">Format of the scheduled report.</span></span> <span data-ttu-id="f030b-173">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="f030b-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="f030b-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="f030b-174">Response</span></span>
<span data-ttu-id="f030b-175">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f030b-175">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f030b-176">Пример</span><span class="sxs-lookup"><span data-stu-id="f030b-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="f030b-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="f030b-177">Request</span></span>
<span data-ttu-id="f030b-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f030b-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
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

### <a name="response"></a><span data-ttu-id="f030b-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="f030b-179">Response</span></span>
<span data-ttu-id="f030b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f030b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




