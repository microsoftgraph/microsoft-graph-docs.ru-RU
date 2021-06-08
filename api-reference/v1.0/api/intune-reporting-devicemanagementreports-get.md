---
title: Get deviceManagementReports
description: Чтение свойств и связей объекта deviceManagementReports.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb9cf59d3bcf42ec0a1fc6a68c7ec0cc65a68579
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758650"
---
# <a name="get-devicemanagementreports"></a><span data-ttu-id="694f2-103">Get deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="694f2-103">Get deviceManagementReports</span></span>

<span data-ttu-id="694f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="694f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="694f2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="694f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="694f2-106">Чтение свойств и связей [объекта deviceManagementReports.](../resources/intune-reporting-devicemanagementreports.md)</span><span class="sxs-lookup"><span data-stu-id="694f2-106">Read properties and relationships of the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="694f2-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="694f2-107">Prerequisites</span></span>
<span data-ttu-id="694f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="694f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="694f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="694f2-110">Permission type</span></span>|<span data-ttu-id="694f2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="694f2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="694f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="694f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="694f2-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="694f2-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="694f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="694f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="694f2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="694f2-115">Not supported.</span></span>|
|<span data-ttu-id="694f2-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="694f2-116">Application</span></span>|<span data-ttu-id="694f2-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="694f2-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="694f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="694f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="694f2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="694f2-119">Optional query parameters</span></span>
<span data-ttu-id="694f2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="694f2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="694f2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="694f2-121">Request headers</span></span>
|<span data-ttu-id="694f2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="694f2-122">Header</span></span>|<span data-ttu-id="694f2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="694f2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="694f2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="694f2-124">Authorization</span></span>|<span data-ttu-id="694f2-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="694f2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="694f2-126">Accept</span><span class="sxs-lookup"><span data-stu-id="694f2-126">Accept</span></span>|<span data-ttu-id="694f2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="694f2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="694f2-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="694f2-128">Request body</span></span>
<span data-ttu-id="694f2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="694f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="694f2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="694f2-130">Response</span></span>
<span data-ttu-id="694f2-131">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="694f2-131">If successful, this method returns a `200 OK` response code and [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="694f2-132">Пример</span><span class="sxs-lookup"><span data-stu-id="694f2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="694f2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="694f2-133">Request</span></span>
<span data-ttu-id="694f2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="694f2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/reports
```

### <a name="response"></a><span data-ttu-id="694f2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="694f2-135">Response</span></span>
<span data-ttu-id="694f2-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="694f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 137

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementReports",
    "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
  }
}
```




