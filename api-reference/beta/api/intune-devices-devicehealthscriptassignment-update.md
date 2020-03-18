---
title: Обновление Девицехеалсскриптассигнмент
description: Обновление свойств объекта Девицехеалсскриптассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7c78f85e1ab8e721985a60f79977213205870f7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769089"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="9ab31-103">Обновление Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="9ab31-103">Update deviceHealthScriptAssignment</span></span>

> <span data-ttu-id="9ab31-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ab31-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9ab31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ab31-106">Обновление свойств объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9ab31-106">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ab31-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9ab31-107">Prerequisites</span></span>
<span data-ttu-id="9ab31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab31-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ab31-110">Permission type</span></span>|<span data-ttu-id="9ab31-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ab31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ab31-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ab31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ab31-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ab31-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9ab31-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ab31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ab31-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ab31-115">Not supported.</span></span>|
|<span data-ttu-id="9ab31-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9ab31-116">Application</span></span>|<span data-ttu-id="9ab31-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ab31-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ab31-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ab31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9ab31-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9ab31-119">Request headers</span></span>
|<span data-ttu-id="9ab31-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9ab31-120">Header</span></span>|<span data-ttu-id="9ab31-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9ab31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ab31-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ab31-122">Authorization</span></span>|<span data-ttu-id="9ab31-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ab31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ab31-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9ab31-124">Accept</span></span>|<span data-ttu-id="9ab31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ab31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ab31-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ab31-126">Request body</span></span>
<span data-ttu-id="9ab31-127">В тексте запроса добавьте представление объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ab31-127">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="9ab31-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9ab31-128">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="9ab31-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ab31-129">Property</span></span>|<span data-ttu-id="9ab31-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9ab31-130">Type</span></span>|<span data-ttu-id="9ab31-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9ab31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ab31-132">id</span><span class="sxs-lookup"><span data-stu-id="9ab31-132">id</span></span>|<span data-ttu-id="9ab31-133">String</span><span class="sxs-lookup"><span data-stu-id="9ab31-133">String</span></span>|<span data-ttu-id="9ab31-134">Ключ объекта назначения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="9ab31-134">Key of the device health script assignment entity.</span></span> <span data-ttu-id="9ab31-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ab31-135">This property is read-only.</span></span>|
|<span data-ttu-id="9ab31-136">target</span><span class="sxs-lookup"><span data-stu-id="9ab31-136">target</span></span>|[<span data-ttu-id="9ab31-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9ab31-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9ab31-138">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="9ab31-138">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="9ab31-139">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="9ab31-139">runRemediationScript</span></span>|<span data-ttu-id="9ab31-140">Логический</span><span class="sxs-lookup"><span data-stu-id="9ab31-140">Boolean</span></span>|<span data-ttu-id="9ab31-141">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="9ab31-141">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="9ab31-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="9ab31-142">runSchedule</span></span>|[<span data-ttu-id="9ab31-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="9ab31-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="9ab31-144">Расписание запуска сценария для целевой группы</span><span class="sxs-lookup"><span data-stu-id="9ab31-144">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="9ab31-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab31-145">Response</span></span>
<span data-ttu-id="9ab31-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9ab31-146">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ab31-147">Пример</span><span class="sxs-lookup"><span data-stu-id="9ab31-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ab31-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ab31-148">Request</span></span>
<span data-ttu-id="9ab31-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ab31-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```

### <a name="response"></a><span data-ttu-id="9ab31-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ab31-150">Response</span></span>
<span data-ttu-id="9ab31-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9ab31-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "c08c4eb1-4eb1-c08c-b14e-8cc0b14e8cc0",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```




