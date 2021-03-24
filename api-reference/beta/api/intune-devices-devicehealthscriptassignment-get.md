---
title: Get deviceHealthScriptAssignment
description: Чтение свойств и связей объекта deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e18a4755898e217e73520c0232de084a23bb6734
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128567"
---
# <a name="get-devicehealthscriptassignment"></a><span data-ttu-id="7d8fa-103">Get deviceHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="7d8fa-103">Get deviceHealthScriptAssignment</span></span>

<span data-ttu-id="7d8fa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d8fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d8fa-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d8fa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d8fa-107">Чтение свойств и связей [объекта deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7d8fa-107">Read properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d8fa-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7d8fa-108">Prerequisites</span></span>
<span data-ttu-id="7d8fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d8fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d8fa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d8fa-111">Permission type</span></span>|<span data-ttu-id="7d8fa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d8fa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d8fa-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d8fa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d8fa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d8fa-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d8fa-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d8fa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d8fa-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-116">Not supported.</span></span>|
|<span data-ttu-id="7d8fa-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d8fa-117">Application</span></span>|<span data-ttu-id="7d8fa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d8fa-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d8fa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d8fa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
GET /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d8fa-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d8fa-120">Optional query parameters</span></span>
<span data-ttu-id="7d8fa-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d8fa-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d8fa-122">Request headers</span></span>
|<span data-ttu-id="7d8fa-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d8fa-123">Header</span></span>|<span data-ttu-id="7d8fa-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7d8fa-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d8fa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d8fa-125">Authorization</span></span>|<span data-ttu-id="7d8fa-126">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d8fa-127">Accept</span><span class="sxs-lookup"><span data-stu-id="7d8fa-127">Accept</span></span>|<span data-ttu-id="7d8fa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d8fa-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d8fa-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d8fa-129">Request body</span></span>
<span data-ttu-id="7d8fa-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d8fa-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d8fa-131">Response</span></span>
<span data-ttu-id="7d8fa-132">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` [объект deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-132">If successful, this method returns a `200 OK` response code and [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d8fa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7d8fa-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d8fa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d8fa-134">Request</span></span>
<span data-ttu-id="7d8fa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

### <a name="response"></a><span data-ttu-id="7d8fa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d8fa-136">Response</span></span>
<span data-ttu-id="7d8fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7d8fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 688

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
    "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
    "target": {
      "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include",
      "collectionId": "Collection Id value"
    },
    "runRemediationScript": true,
    "runSchedule": {
      "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
      "interval": 8,
      "useUtc": true,
      "time": "11:58:36.2550000"
    }
  }
}
```




