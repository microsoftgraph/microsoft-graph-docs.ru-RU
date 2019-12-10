---
title: Создание Девицеманажементрепортсчедуле
description: Создание нового объекта Девицеманажементрепортсчедуле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5cac3be06db06eb13fc371c41fe832dabefd36dd
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940266"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="cbc9b-103">Создание Девицеманажементрепортсчедуле</span><span class="sxs-lookup"><span data-stu-id="cbc9b-103">Create deviceManagementReportSchedule</span></span>

> <span data-ttu-id="cbc9b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbc9b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbc9b-106">Создание нового объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="cbc9b-106">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbc9b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cbc9b-107">Prerequisites</span></span>
<span data-ttu-id="cbc9b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbc9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbc9b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbc9b-110">Permission type</span></span>|<span data-ttu-id="cbc9b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbc9b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbc9b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbc9b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbc9b-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cbc9b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cbc9b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbc9b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbc9b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-115">Not supported.</span></span>|
|<span data-ttu-id="cbc9b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbc9b-116">Application</span></span>|<span data-ttu-id="cbc9b-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="cbc9b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbc9b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbc9b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="cbc9b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cbc9b-119">Request headers</span></span>
|<span data-ttu-id="cbc9b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbc9b-120">Header</span></span>|<span data-ttu-id="cbc9b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cbc9b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbc9b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbc9b-122">Authorization</span></span>|<span data-ttu-id="cbc9b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbc9b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cbc9b-124">Accept</span></span>|<span data-ttu-id="cbc9b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbc9b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbc9b-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cbc9b-126">Request body</span></span>
<span data-ttu-id="cbc9b-127">В тексте запроса добавьте представление объекта Девицеманажементрепортсчедуле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-127">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="cbc9b-128">В следующей таблице приведены свойства, необходимые при создании Девицеманажементрепортсчедуле.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-128">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="cbc9b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbc9b-129">Property</span></span>|<span data-ttu-id="cbc9b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cbc9b-130">Type</span></span>|<span data-ttu-id="cbc9b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cbc9b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbc9b-132">id</span><span class="sxs-lookup"><span data-stu-id="cbc9b-132">id</span></span>|<span data-ttu-id="cbc9b-133">Строка</span><span class="sxs-lookup"><span data-stu-id="cbc9b-133">String</span></span>|<span data-ttu-id="cbc9b-134">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="cbc9b-134">Unique identifier for this entity</span></span>|
|<span data-ttu-id="cbc9b-135">репортсчедуленаме</span><span class="sxs-lookup"><span data-stu-id="cbc9b-135">reportScheduleName</span></span>|<span data-ttu-id="cbc9b-136">Строка</span><span class="sxs-lookup"><span data-stu-id="cbc9b-136">String</span></span>|<span data-ttu-id="cbc9b-137">Имя расписания</span><span class="sxs-lookup"><span data-stu-id="cbc9b-137">Name of the schedule</span></span>|
|<span data-ttu-id="cbc9b-138">subject</span><span class="sxs-lookup"><span data-stu-id="cbc9b-138">subject</span></span>|<span data-ttu-id="cbc9b-139">String</span><span class="sxs-lookup"><span data-stu-id="cbc9b-139">String</span></span>|<span data-ttu-id="cbc9b-140">Тема запланированных отчетов, которые доставляются</span><span class="sxs-lookup"><span data-stu-id="cbc9b-140">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="cbc9b-141">письма</span><span class="sxs-lookup"><span data-stu-id="cbc9b-141">emails</span></span>|<span data-ttu-id="cbc9b-142">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cbc9b-142">String collection</span></span>|<span data-ttu-id="cbc9b-143">Сообщения электронной почты, на которые доставляются запланированные отчеты</span><span class="sxs-lookup"><span data-stu-id="cbc9b-143">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="cbc9b-144">recurrence</span><span class="sxs-lookup"><span data-stu-id="cbc9b-144">recurrence</span></span>|[<span data-ttu-id="cbc9b-145">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="cbc9b-145">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="cbc9b-146">Периодичность запланированной доставки отчета.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-146">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="cbc9b-147">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-147">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="cbc9b-148">startDateTime</span><span class="sxs-lookup"><span data-stu-id="cbc9b-148">startDateTime</span></span>|<span data-ttu-id="cbc9b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbc9b-149">DateTimeOffset</span></span>|<span data-ttu-id="cbc9b-150">Время, когда начинается доставка запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="cbc9b-150">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="cbc9b-151">endDateTime</span><span class="sxs-lookup"><span data-stu-id="cbc9b-151">endDateTime</span></span>|<span data-ttu-id="cbc9b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbc9b-152">DateTimeOffset</span></span>|<span data-ttu-id="cbc9b-153">Время окончания доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="cbc9b-153">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="cbc9b-154">userId</span><span class="sxs-lookup"><span data-stu-id="cbc9b-154">userId</span></span>|<span data-ttu-id="cbc9b-155">String</span><span class="sxs-lookup"><span data-stu-id="cbc9b-155">String</span></span>|<span data-ttu-id="cbc9b-156">Идентификатор пользователя, создавшего отчет</span><span class="sxs-lookup"><span data-stu-id="cbc9b-156">The Id of the User who created the report</span></span>|
|<span data-ttu-id="cbc9b-157">репортнаме</span><span class="sxs-lookup"><span data-stu-id="cbc9b-157">reportName</span></span>|<span data-ttu-id="cbc9b-158">Строка</span><span class="sxs-lookup"><span data-stu-id="cbc9b-158">String</span></span>|<span data-ttu-id="cbc9b-159">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="cbc9b-159">Name of the report</span></span>|
|<span data-ttu-id="cbc9b-160">filter</span><span class="sxs-lookup"><span data-stu-id="cbc9b-160">filter</span></span>|<span data-ttu-id="cbc9b-161">Строка</span><span class="sxs-lookup"><span data-stu-id="cbc9b-161">String</span></span>|<span data-ttu-id="cbc9b-162">Фильтры, примененные к отчету</span><span class="sxs-lookup"><span data-stu-id="cbc9b-162">Filters applied on the report</span></span>|
|<span data-ttu-id="cbc9b-163">select</span><span class="sxs-lookup"><span data-stu-id="cbc9b-163">select</span></span>|<span data-ttu-id="cbc9b-164">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cbc9b-164">String collection</span></span>|<span data-ttu-id="cbc9b-165">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="cbc9b-165">Columns selected from the report</span></span>|
|<span data-ttu-id="cbc9b-166">orderBy</span><span class="sxs-lookup"><span data-stu-id="cbc9b-166">orderBy</span></span>|<span data-ttu-id="cbc9b-167">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="cbc9b-167">String collection</span></span>|<span data-ttu-id="cbc9b-168">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="cbc9b-168">Ordering of columns in the report</span></span>|
|<span data-ttu-id="cbc9b-169">format</span><span class="sxs-lookup"><span data-stu-id="cbc9b-169">format</span></span>|[<span data-ttu-id="cbc9b-170">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="cbc9b-170">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="cbc9b-171">Формат запланированного отчета.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-171">Format of the scheduled report.</span></span> <span data-ttu-id="cbc9b-172">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-172">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="cbc9b-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc9b-173">Response</span></span>
<span data-ttu-id="cbc9b-174">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-174">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbc9b-175">Пример</span><span class="sxs-lookup"><span data-stu-id="cbc9b-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbc9b-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbc9b-176">Request</span></span>
<span data-ttu-id="cbc9b-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cbc9b-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbc9b-178">Response</span></span>
<span data-ttu-id="cbc9b-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbc9b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





