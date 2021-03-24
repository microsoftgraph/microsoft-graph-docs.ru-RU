---
title: Список deviceManagementCachedReportConfigurations
description: Список свойств и связей объектов deviceManagementCachedReportConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 303debd9d6de4524667a573f2608204e5fdffdd8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123408"
---
# <a name="list-devicemanagementcachedreportconfigurations"></a><span data-ttu-id="8cd20-103">Список deviceManagementCachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="8cd20-103">List deviceManagementCachedReportConfigurations</span></span>

<span data-ttu-id="8cd20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cd20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cd20-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cd20-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cd20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cd20-107">Список свойств и связей [объектов deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8cd20-107">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cd20-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8cd20-108">Prerequisites</span></span>
<span data-ttu-id="8cd20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cd20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cd20-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd20-111">Permission type</span></span>|<span data-ttu-id="8cd20-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cd20-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cd20-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cd20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cd20-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd20-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8cd20-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cd20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cd20-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd20-116">Not supported.</span></span>|
|<span data-ttu-id="8cd20-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8cd20-117">Application</span></span>|<span data-ttu-id="8cd20-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd20-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cd20-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cd20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8cd20-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8cd20-120">Request headers</span></span>
|<span data-ttu-id="8cd20-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8cd20-121">Header</span></span>|<span data-ttu-id="8cd20-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8cd20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cd20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cd20-123">Authorization</span></span>|<span data-ttu-id="8cd20-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cd20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cd20-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8cd20-125">Accept</span></span>|<span data-ttu-id="8cd20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cd20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cd20-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cd20-127">Request body</span></span>
<span data-ttu-id="8cd20-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8cd20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cd20-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd20-129">Response</span></span>
<span data-ttu-id="8cd20-130">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8cd20-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cd20-131">Пример</span><span class="sxs-lookup"><span data-stu-id="8cd20-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cd20-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cd20-132">Request</span></span>
<span data-ttu-id="8cd20-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cd20-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
```

### <a name="response"></a><span data-ttu-id="8cd20-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd20-134">Response</span></span>
<span data-ttu-id="8cd20-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8cd20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 556

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
      "id": "46947722-7722-4694-2277-944622779446",
      "reportName": "Report Name value",
      "filter": "Filter value",
      "select": [
        "Select value"
      ],
      "orderBy": [
        "Order By value"
      ],
      "metadata": "Metadata value",
      "status": "notStarted",
      "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
    }
  ]
}
```




