---
title: Получение Девицеманажементрепортсчедуле
description: Чтение свойств и связей объекта Девицеманажементрепортсчедуле.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 458d101cd3f60a2771f29aa1c6b103a6ce547373
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801336"
---
# <a name="get-devicemanagementreportschedule"></a><span data-ttu-id="fda14-103">Получение Девицеманажементрепортсчедуле</span><span class="sxs-lookup"><span data-stu-id="fda14-103">Get deviceManagementReportSchedule</span></span>

> <span data-ttu-id="fda14-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fda14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fda14-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fda14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fda14-106">Чтение свойств и связей объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="fda14-106">Read properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fda14-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fda14-107">Prerequisites</span></span>
<span data-ttu-id="fda14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fda14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fda14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fda14-110">Permission type</span></span>|<span data-ttu-id="fda14-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fda14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fda14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fda14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fda14-113">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fda14-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fda14-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fda14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fda14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fda14-115">Not supported.</span></span>|
|<span data-ttu-id="fda14-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="fda14-116">Application</span></span>|<span data-ttu-id="fda14-117">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="fda14-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fda14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fda14-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fda14-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fda14-119">Optional query parameters</span></span>
<span data-ttu-id="fda14-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fda14-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fda14-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fda14-121">Request headers</span></span>
|<span data-ttu-id="fda14-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fda14-122">Header</span></span>|<span data-ttu-id="fda14-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fda14-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fda14-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fda14-124">Authorization</span></span>|<span data-ttu-id="fda14-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fda14-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fda14-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fda14-126">Accept</span></span>|<span data-ttu-id="fda14-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fda14-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fda14-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fda14-128">Request body</span></span>
<span data-ttu-id="fda14-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fda14-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fda14-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fda14-130">Response</span></span>
<span data-ttu-id="fda14-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fda14-131">If successful, this method returns a `200 OK` response code and [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fda14-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fda14-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="fda14-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fda14-133">Request</span></span>
<span data-ttu-id="fda14-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fda14-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

### <a name="response"></a><span data-ttu-id="fda14-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fda14-135">Response</span></span>
<span data-ttu-id="fda14-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fda14-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 647

{
  "value": {
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
}
```




