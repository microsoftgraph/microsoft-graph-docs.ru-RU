---
title: Создание Девицеманажементрепортсчедуле
description: Создание нового объекта Девицеманажементрепортсчедуле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f91038e518550b9ebfc50d59c3a0168d8e489cd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49257627"
---
# <a name="create-devicemanagementreportschedule"></a><span data-ttu-id="c82cf-103">Создание Девицеманажементрепортсчедуле</span><span class="sxs-lookup"><span data-stu-id="c82cf-103">Create deviceManagementReportSchedule</span></span>

<span data-ttu-id="c82cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c82cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c82cf-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c82cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c82cf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c82cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c82cf-107">Создание нового объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="c82cf-107">Create a new [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c82cf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c82cf-108">Prerequisites</span></span>
<span data-ttu-id="c82cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c82cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c82cf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c82cf-111">Permission type</span></span>|<span data-ttu-id="c82cf-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c82cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c82cf-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c82cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c82cf-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c82cf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c82cf-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c82cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c82cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c82cf-116">Not supported.</span></span>|
|<span data-ttu-id="c82cf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c82cf-117">Application</span></span>|<span data-ttu-id="c82cf-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementManagedDevices. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c82cf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c82cf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c82cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="c82cf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c82cf-120">Request headers</span></span>
|<span data-ttu-id="c82cf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c82cf-121">Header</span></span>|<span data-ttu-id="c82cf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c82cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c82cf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c82cf-123">Authorization</span></span>|<span data-ttu-id="c82cf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c82cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c82cf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c82cf-125">Accept</span></span>|<span data-ttu-id="c82cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c82cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c82cf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c82cf-127">Request body</span></span>
<span data-ttu-id="c82cf-128">В тексте запроса добавьте представление объекта Девицеманажементрепортсчедуле в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c82cf-128">In the request body, supply a JSON representation for the deviceManagementReportSchedule object.</span></span>

<span data-ttu-id="c82cf-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементрепортсчедуле.</span><span class="sxs-lookup"><span data-stu-id="c82cf-129">The following table shows the properties that are required when you create the deviceManagementReportSchedule.</span></span>

|<span data-ttu-id="c82cf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c82cf-130">Property</span></span>|<span data-ttu-id="c82cf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c82cf-131">Type</span></span>|<span data-ttu-id="c82cf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c82cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c82cf-133">id</span><span class="sxs-lookup"><span data-stu-id="c82cf-133">id</span></span>|<span data-ttu-id="c82cf-134">String</span><span class="sxs-lookup"><span data-stu-id="c82cf-134">String</span></span>|<span data-ttu-id="c82cf-135">Уникальный идентификатор для этой сущности</span><span class="sxs-lookup"><span data-stu-id="c82cf-135">Unique identifier for this entity</span></span>|
|<span data-ttu-id="c82cf-136">репортсчедуленаме</span><span class="sxs-lookup"><span data-stu-id="c82cf-136">reportScheduleName</span></span>|<span data-ttu-id="c82cf-137">String</span><span class="sxs-lookup"><span data-stu-id="c82cf-137">String</span></span>|<span data-ttu-id="c82cf-138">Имя расписания</span><span class="sxs-lookup"><span data-stu-id="c82cf-138">Name of the schedule</span></span>|
|<span data-ttu-id="c82cf-139">subject</span><span class="sxs-lookup"><span data-stu-id="c82cf-139">subject</span></span>|<span data-ttu-id="c82cf-140">String</span><span class="sxs-lookup"><span data-stu-id="c82cf-140">String</span></span>|<span data-ttu-id="c82cf-141">Тема запланированных отчетов, которые доставляются</span><span class="sxs-lookup"><span data-stu-id="c82cf-141">Subject of the scheduled reports that are delivered</span></span>|
|<span data-ttu-id="c82cf-142">письма</span><span class="sxs-lookup"><span data-stu-id="c82cf-142">emails</span></span>|<span data-ttu-id="c82cf-143">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c82cf-143">String collection</span></span>|<span data-ttu-id="c82cf-144">Сообщения электронной почты, на которые доставляются запланированные отчеты</span><span class="sxs-lookup"><span data-stu-id="c82cf-144">Emails to which the scheduled reports are delivered</span></span>|
|<span data-ttu-id="c82cf-145">recurrence</span><span class="sxs-lookup"><span data-stu-id="c82cf-145">recurrence</span></span>|[<span data-ttu-id="c82cf-146">deviceManagementScheduledReportRecurrence</span><span class="sxs-lookup"><span data-stu-id="c82cf-146">deviceManagementScheduledReportRecurrence</span></span>](../resources/intune-reporting-devicemanagementscheduledreportrecurrence.md)|<span data-ttu-id="c82cf-147">Периодичность запланированной доставки отчета.</span><span class="sxs-lookup"><span data-stu-id="c82cf-147">Frequency of scheduled report delivery.</span></span> <span data-ttu-id="c82cf-148">Возможные значения: `none`, `daily`, `weekly`, `monthly`.</span><span class="sxs-lookup"><span data-stu-id="c82cf-148">Possible values are: `none`, `daily`, `weekly`, `monthly`.</span></span>|
|<span data-ttu-id="c82cf-149">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c82cf-149">startDateTime</span></span>|<span data-ttu-id="c82cf-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c82cf-150">DateTimeOffset</span></span>|<span data-ttu-id="c82cf-151">Время, когда начинается доставка запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="c82cf-151">Time that the delivery of the scheduled reports starts</span></span>|
|<span data-ttu-id="c82cf-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c82cf-152">endDateTime</span></span>|<span data-ttu-id="c82cf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c82cf-153">DateTimeOffset</span></span>|<span data-ttu-id="c82cf-154">Время окончания доставки запланированных отчетов</span><span class="sxs-lookup"><span data-stu-id="c82cf-154">Time that the delivery of the scheduled reports ends</span></span>|
|<span data-ttu-id="c82cf-155">userId</span><span class="sxs-lookup"><span data-stu-id="c82cf-155">userId</span></span>|<span data-ttu-id="c82cf-156">String</span><span class="sxs-lookup"><span data-stu-id="c82cf-156">String</span></span>|<span data-ttu-id="c82cf-157">Идентификатор пользователя, создавшего отчет</span><span class="sxs-lookup"><span data-stu-id="c82cf-157">The Id of the User who created the report</span></span>|
|<span data-ttu-id="c82cf-158">репортнаме</span><span class="sxs-lookup"><span data-stu-id="c82cf-158">reportName</span></span>|<span data-ttu-id="c82cf-159">String</span><span class="sxs-lookup"><span data-stu-id="c82cf-159">String</span></span>|<span data-ttu-id="c82cf-160">Имя отчета</span><span class="sxs-lookup"><span data-stu-id="c82cf-160">Name of the report</span></span>|
|<span data-ttu-id="c82cf-161">filter</span><span class="sxs-lookup"><span data-stu-id="c82cf-161">filter</span></span>|<span data-ttu-id="c82cf-162">String</span><span class="sxs-lookup"><span data-stu-id="c82cf-162">String</span></span>|<span data-ttu-id="c82cf-163">Фильтры, примененные к отчету</span><span class="sxs-lookup"><span data-stu-id="c82cf-163">Filters applied on the report</span></span>|
|<span data-ttu-id="c82cf-164">select</span><span class="sxs-lookup"><span data-stu-id="c82cf-164">select</span></span>|<span data-ttu-id="c82cf-165">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c82cf-165">String collection</span></span>|<span data-ttu-id="c82cf-166">Столбцы, выбранные из отчета</span><span class="sxs-lookup"><span data-stu-id="c82cf-166">Columns selected from the report</span></span>|
|<span data-ttu-id="c82cf-167">orderBy</span><span class="sxs-lookup"><span data-stu-id="c82cf-167">orderBy</span></span>|<span data-ttu-id="c82cf-168">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="c82cf-168">String collection</span></span>|<span data-ttu-id="c82cf-169">Упорядочение столбцов в отчете</span><span class="sxs-lookup"><span data-stu-id="c82cf-169">Ordering of columns in the report</span></span>|
|<span data-ttu-id="c82cf-170">format</span><span class="sxs-lookup"><span data-stu-id="c82cf-170">format</span></span>|[<span data-ttu-id="c82cf-171">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="c82cf-171">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="c82cf-172">Формат запланированного отчета.</span><span class="sxs-lookup"><span data-stu-id="c82cf-172">Format of the scheduled report.</span></span> <span data-ttu-id="c82cf-173">Возможные значения: `csv`, `pdf`.</span><span class="sxs-lookup"><span data-stu-id="c82cf-173">Possible values are: `csv`, `pdf`.</span></span>|



## <a name="response"></a><span data-ttu-id="c82cf-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c82cf-174">Response</span></span>
<span data-ttu-id="c82cf-175">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c82cf-175">If successful, this method returns a `201 Created` response code and a [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c82cf-176">Пример</span><span class="sxs-lookup"><span data-stu-id="c82cf-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="c82cf-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="c82cf-177">Request</span></span>
<span data-ttu-id="c82cf-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c82cf-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c82cf-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="c82cf-179">Response</span></span>
<span data-ttu-id="c82cf-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c82cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




