---
title: Получение Девицеманажементрепортсчедуле
description: Чтение свойств и связей объекта Девицеманажементрепортсчедуле.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 17f605dfdc69bbb226227cad961e1e96e15554bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47969559"
---
# <a name="get-devicemanagementreportschedule"></a><span data-ttu-id="aaa01-103">Получение Девицеманажементрепортсчедуле</span><span class="sxs-lookup"><span data-stu-id="aaa01-103">Get deviceManagementReportSchedule</span></span>

<span data-ttu-id="aaa01-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaa01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aaa01-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaa01-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aaa01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaa01-107">Чтение свойств и связей объекта [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="aaa01-107">Read properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaa01-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="aaa01-108">Prerequisites</span></span>
<span data-ttu-id="aaa01-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaa01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaa01-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaa01-111">Permission type</span></span>|<span data-ttu-id="aaa01-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaa01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaa01-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaa01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaa01-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="aaa01-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="aaa01-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaa01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaa01-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaa01-116">Not supported.</span></span>|
|<span data-ttu-id="aaa01-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaa01-117">Application</span></span>|<span data-ttu-id="aaa01-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="aaa01-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaa01-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaa01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaa01-120">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="aaa01-120">Optional query parameters</span></span>
<span data-ttu-id="aaa01-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aaa01-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaa01-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaa01-122">Request headers</span></span>
|<span data-ttu-id="aaa01-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aaa01-123">Header</span></span>|<span data-ttu-id="aaa01-124">Значение</span><span class="sxs-lookup"><span data-stu-id="aaa01-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaa01-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaa01-125">Authorization</span></span>|<span data-ttu-id="aaa01-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aaa01-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaa01-127">Accept</span><span class="sxs-lookup"><span data-stu-id="aaa01-127">Accept</span></span>|<span data-ttu-id="aaa01-128">application/json</span><span class="sxs-lookup"><span data-stu-id="aaa01-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaa01-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aaa01-129">Request body</span></span>
<span data-ttu-id="aaa01-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aaa01-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaa01-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa01-131">Response</span></span>
<span data-ttu-id="aaa01-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aaa01-132">If successful, this method returns a `200 OK` response code and [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaa01-133">Пример</span><span class="sxs-lookup"><span data-stu-id="aaa01-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaa01-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaa01-134">Request</span></span>
<span data-ttu-id="aaa01-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaa01-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

### <a name="response"></a><span data-ttu-id="aaa01-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaa01-136">Response</span></span>
<span data-ttu-id="aaa01-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaa01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






