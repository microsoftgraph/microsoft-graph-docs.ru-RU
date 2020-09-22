---
title: Список Девицехеалсскриптассигнментс
description: Список свойств и связей объектов Девицехеалсскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 84b9206937509d034a6df44dfb59a593d9475a71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050712"
---
# <a name="list-devicehealthscriptassignments"></a><span data-ttu-id="5e038-103">Список Девицехеалсскриптассигнментс</span><span class="sxs-lookup"><span data-stu-id="5e038-103">List deviceHealthScriptAssignments</span></span>

<span data-ttu-id="5e038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e038-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5e038-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e038-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e038-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e038-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e038-107">Список свойств и связей объектов [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5e038-107">List properties and relationships of the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e038-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5e038-108">Prerequisites</span></span>
<span data-ttu-id="5e038-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e038-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e038-111">Permission type</span></span>|<span data-ttu-id="5e038-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e038-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e038-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e038-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e038-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e038-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5e038-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e038-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e038-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e038-116">Not supported.</span></span>|
|<span data-ttu-id="5e038-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e038-117">Application</span></span>|<span data-ttu-id="5e038-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e038-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e038-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e038-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
GET /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5e038-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5e038-120">Request headers</span></span>
|<span data-ttu-id="5e038-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e038-121">Header</span></span>|<span data-ttu-id="5e038-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e038-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e038-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e038-123">Authorization</span></span>|<span data-ttu-id="5e038-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e038-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e038-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e038-125">Accept</span></span>|<span data-ttu-id="5e038-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e038-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e038-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e038-127">Request body</span></span>
<span data-ttu-id="5e038-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5e038-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e038-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e038-129">Response</span></span>
<span data-ttu-id="5e038-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5e038-130">If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e038-131">Пример</span><span class="sxs-lookup"><span data-stu-id="5e038-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e038-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e038-132">Request</span></span>
<span data-ttu-id="5e038-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e038-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

### <a name="response"></a><span data-ttu-id="5e038-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e038-134">Response</span></span>
<span data-ttu-id="5e038-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e038-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 664

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
      "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      },
      "runRemediationScript": true,
      "runSchedule": {
        "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule",
        "interval": 8,
        "useUtc": true,
        "time": "11:58:36.2550000"
      }
    }
  ]
}
```






