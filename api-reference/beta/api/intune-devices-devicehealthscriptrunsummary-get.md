---
title: Get deviceHealthScriptRunSummary
description: Чтение свойств и связей объекта deviceHealthScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b31b33a3d3243aee2ff600b4bf5ff7c9ffb671ae
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665534"
---
# <a name="get-devicehealthscriptrunsummary"></a><span data-ttu-id="46a2f-103">Get deviceHealthScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="46a2f-103">Get deviceHealthScriptRunSummary</span></span>

<span data-ttu-id="46a2f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46a2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46a2f-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46a2f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46a2f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46a2f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46a2f-107">Чтение свойств и связей [объекта deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="46a2f-107">Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46a2f-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46a2f-108">Prerequisites</span></span>
<span data-ttu-id="46a2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46a2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46a2f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46a2f-111">Permission type</span></span>|<span data-ttu-id="46a2f-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46a2f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46a2f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46a2f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46a2f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a2f-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="46a2f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46a2f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46a2f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46a2f-116">Not supported.</span></span>|
|<span data-ttu-id="46a2f-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="46a2f-117">Application</span></span>|<span data-ttu-id="46a2f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46a2f-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46a2f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46a2f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46a2f-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="46a2f-120">Optional query parameters</span></span>
<span data-ttu-id="46a2f-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="46a2f-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="46a2f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46a2f-122">Request headers</span></span>
|<span data-ttu-id="46a2f-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46a2f-123">Header</span></span>|<span data-ttu-id="46a2f-124">Значение</span><span class="sxs-lookup"><span data-stu-id="46a2f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46a2f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="46a2f-125">Authorization</span></span>|<span data-ttu-id="46a2f-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46a2f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46a2f-127">Accept</span><span class="sxs-lookup"><span data-stu-id="46a2f-127">Accept</span></span>|<span data-ttu-id="46a2f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="46a2f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46a2f-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46a2f-129">Request body</span></span>
<span data-ttu-id="46a2f-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46a2f-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46a2f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="46a2f-131">Response</span></span>
<span data-ttu-id="46a2f-132">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="46a2f-132">If successful, this method returns a `200 OK` response code and [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46a2f-133">Пример</span><span class="sxs-lookup"><span data-stu-id="46a2f-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="46a2f-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="46a2f-134">Request</span></span>
<span data-ttu-id="46a2f-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46a2f-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

### <a name="response"></a><span data-ttu-id="46a2f-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="46a2f-136">Response</span></span>
<span data-ttu-id="46a2f-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46a2f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
    "id": "8221b043-b043-8221-43b0-218243b02182",
    "noIssueDetectedDeviceCount": 10,
    "issueDetectedDeviceCount": 8,
    "detectionScriptErrorDeviceCount": 15,
    "detectionScriptPendingDeviceCount": 1,
    "detectionScriptNotApplicableDeviceCount": 7,
    "issueRemediatedDeviceCount": 10,
    "remediationSkippedDeviceCount": 13,
    "issueReoccurredDeviceCount": 10,
    "remediationScriptErrorDeviceCount": 1,
    "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
    "issueRemediatedCumulativeDeviceCount": 4
  }
}
```




