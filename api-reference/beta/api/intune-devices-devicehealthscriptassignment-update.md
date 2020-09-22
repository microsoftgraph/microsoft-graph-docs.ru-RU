---
title: Обновление Девицехеалсскриптассигнмент
description: Обновление свойств объекта Девицехеалсскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 96b22d18a641f5f50eb1afff5a7774b7fc37f8d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986639"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="fbc4c-103">Обновление Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="fbc4c-103">Update deviceHealthScriptAssignment</span></span>

<span data-ttu-id="fbc4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbc4c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc4c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc4c-107">Обновление свойств объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="fbc4c-107">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fbc4c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fbc4c-108">Prerequisites</span></span>
<span data-ttu-id="fbc4c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fbc4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbc4c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fbc4c-111">Permission type</span></span>|<span data-ttu-id="fbc4c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fbc4c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fbc4c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fbc4c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fbc4c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbc4c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fbc4c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fbc4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fbc4c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-116">Not supported.</span></span>|
|<span data-ttu-id="fbc4c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fbc4c-117">Application</span></span>|<span data-ttu-id="fbc4c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fbc4c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fbc4c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fbc4c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fbc4c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fbc4c-120">Request headers</span></span>
|<span data-ttu-id="fbc4c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fbc4c-121">Header</span></span>|<span data-ttu-id="fbc4c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fbc4c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fbc4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fbc4c-123">Authorization</span></span>|<span data-ttu-id="fbc4c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fbc4c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fbc4c-125">Accept</span></span>|<span data-ttu-id="fbc4c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fbc4c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fbc4c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fbc4c-127">Request body</span></span>
<span data-ttu-id="fbc4c-128">В тексте запроса добавьте представление объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-128">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="fbc4c-129">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fbc4c-129">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="fbc4c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbc4c-130">Property</span></span>|<span data-ttu-id="fbc4c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fbc4c-131">Type</span></span>|<span data-ttu-id="fbc4c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fbc4c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc4c-133">id</span><span class="sxs-lookup"><span data-stu-id="fbc4c-133">id</span></span>|<span data-ttu-id="fbc4c-134">String</span><span class="sxs-lookup"><span data-stu-id="fbc4c-134">String</span></span>|<span data-ttu-id="fbc4c-135">Ключ объекта назначения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="fbc4c-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-136">This property is read-only.</span></span>|
|<span data-ttu-id="fbc4c-137">target</span><span class="sxs-lookup"><span data-stu-id="fbc4c-137">target</span></span>|[<span data-ttu-id="fbc4c-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fbc4c-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fbc4c-139">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="fbc4c-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="fbc4c-140">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="fbc4c-140">runRemediationScript</span></span>|<span data-ttu-id="fbc4c-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbc4c-141">Boolean</span></span>|<span data-ttu-id="fbc4c-142">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="fbc4c-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="fbc4c-143">runSchedule</span></span>|[<span data-ttu-id="fbc4c-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="fbc4c-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="fbc4c-145">Расписание запуска сценария для целевой группы</span><span class="sxs-lookup"><span data-stu-id="fbc4c-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="fbc4c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbc4c-146">Response</span></span>
<span data-ttu-id="fbc4c-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-147">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbc4c-148">Пример</span><span class="sxs-lookup"><span data-stu-id="fbc4c-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="fbc4c-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="fbc4c-149">Request</span></span>
<span data-ttu-id="fbc4c-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
Content-type: application/json
Content-length: 526

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
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
```

### <a name="response"></a><span data-ttu-id="fbc4c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="fbc4c-151">Response</span></span>
<span data-ttu-id="fbc4c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fbc4c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

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
```






