---
title: Список Девицеманажементкачедрепортконфигуратионс
description: Список свойств и связей объектов Девицеманажементкачедрепортконфигуратион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 072068fb67b44e5ebf8845d7edda2996090b4011
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445179"
---
# <a name="list-devicemanagementcachedreportconfigurations"></a><span data-ttu-id="876a1-103">Список Девицеманажементкачедрепортконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="876a1-103">List deviceManagementCachedReportConfigurations</span></span>

<span data-ttu-id="876a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="876a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="876a1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="876a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="876a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="876a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="876a1-107">Список свойств и связей объектов [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="876a1-107">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="876a1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="876a1-108">Prerequisites</span></span>
<span data-ttu-id="876a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="876a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="876a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="876a1-111">Permission type</span></span>|<span data-ttu-id="876a1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="876a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="876a1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="876a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="876a1-114">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="876a1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="876a1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="876a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="876a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="876a1-116">Not supported.</span></span>|
|<span data-ttu-id="876a1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="876a1-117">Application</span></span>|<span data-ttu-id="876a1-118">DeviceManagementConfiguration. ReadWrite. ALL, DeviceManagementConfiguration. Read. ALL, DeviceManagementApps. ReadWrite. ALL, DeviceManagementApps. Read. ALL, DeviceManagementManagedDevices. ReadWrite. ALL, DeviceManagementManagedDevices. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="876a1-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="876a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="876a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="876a1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="876a1-120">Request headers</span></span>
|<span data-ttu-id="876a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="876a1-121">Header</span></span>|<span data-ttu-id="876a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="876a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="876a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="876a1-123">Authorization</span></span>|<span data-ttu-id="876a1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="876a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="876a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="876a1-125">Accept</span></span>|<span data-ttu-id="876a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="876a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="876a1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="876a1-127">Request body</span></span>
<span data-ttu-id="876a1-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="876a1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="876a1-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="876a1-129">Response</span></span>
<span data-ttu-id="876a1-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицеманажементкачедрепортконфигуратион](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="876a1-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="876a1-131">Пример</span><span class="sxs-lookup"><span data-stu-id="876a1-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="876a1-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="876a1-132">Request</span></span>
<span data-ttu-id="876a1-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="876a1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
```

### <a name="response"></a><span data-ttu-id="876a1-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="876a1-134">Response</span></span>
<span data-ttu-id="876a1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="876a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 519

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
      "status": "notStarted",
      "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
    }
  ]
}
```



