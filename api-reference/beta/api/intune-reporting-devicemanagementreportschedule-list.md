---
title: Список Девицеманажементрепортсчедулес
description: Список свойств и связей объектов Девицеманажементрепортсчедуле.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ec0473da4ffa8c9808e5595695d397a3d4dabf9d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459074"
---
# <a name="list-devicemanagementreportschedules"></a><span data-ttu-id="09d58-103">Список Девицеманажементрепортсчедулес</span><span class="sxs-lookup"><span data-stu-id="09d58-103">List deviceManagementReportSchedules</span></span>

<span data-ttu-id="09d58-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09d58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09d58-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09d58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09d58-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09d58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09d58-107">Список свойств и связей объектов [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) .</span><span class="sxs-lookup"><span data-stu-id="09d58-107">List properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09d58-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="09d58-108">Prerequisites</span></span>
<span data-ttu-id="09d58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09d58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="09d58-111">Permission type</span></span>|<span data-ttu-id="09d58-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="09d58-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09d58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="09d58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09d58-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="09d58-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="09d58-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="09d58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09d58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09d58-116">Not supported.</span></span>|
|<span data-ttu-id="09d58-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="09d58-117">Application</span></span>|<span data-ttu-id="09d58-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="09d58-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09d58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="09d58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="09d58-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="09d58-120">Request headers</span></span>
|<span data-ttu-id="09d58-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="09d58-121">Header</span></span>|<span data-ttu-id="09d58-122">Значение</span><span class="sxs-lookup"><span data-stu-id="09d58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09d58-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09d58-123">Authorization</span></span>|<span data-ttu-id="09d58-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="09d58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09d58-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09d58-125">Accept</span></span>|<span data-ttu-id="09d58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09d58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09d58-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="09d58-127">Request body</span></span>
<span data-ttu-id="09d58-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="09d58-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09d58-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="09d58-129">Response</span></span>
<span data-ttu-id="09d58-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементрепортсчедуле](../resources/intune-reporting-devicemanagementreportschedule.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="09d58-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09d58-131">Пример</span><span class="sxs-lookup"><span data-stu-id="09d58-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="09d58-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="09d58-132">Request</span></span>
<span data-ttu-id="09d58-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="09d58-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
```

### <a name="response"></a><span data-ttu-id="09d58-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="09d58-134">Response</span></span>
<span data-ttu-id="09d58-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="09d58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 701

{
  "value": [
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
  ]
}
```





