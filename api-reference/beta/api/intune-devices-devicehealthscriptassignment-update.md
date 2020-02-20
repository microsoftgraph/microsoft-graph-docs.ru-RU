---
title: Обновление Девицехеалсскриптассигнмент
description: Обновление свойств объекта Девицехеалсскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa8fd4ee7849d099394266fbe35c7241354fbedb
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162150"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="3fb3d-103">Обновление Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="3fb3d-103">Update deviceHealthScriptAssignment</span></span>

> <span data-ttu-id="3fb3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fb3d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fb3d-106">Обновление свойств объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3fb3d-106">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fb3d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3fb3d-107">Prerequisites</span></span>
<span data-ttu-id="3fb3d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fb3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fb3d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fb3d-110">Permission type</span></span>|<span data-ttu-id="3fb3d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fb3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fb3d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fb3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3fb3d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fb3d-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3fb3d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fb3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fb3d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-115">Not supported.</span></span>|
|<span data-ttu-id="3fb3d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3fb3d-116">Application</span></span>|<span data-ttu-id="3fb3d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fb3d-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fb3d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fb3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3fb3d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3fb3d-119">Request headers</span></span>
|<span data-ttu-id="3fb3d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3fb3d-120">Header</span></span>|<span data-ttu-id="3fb3d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3fb3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fb3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fb3d-122">Authorization</span></span>|<span data-ttu-id="3fb3d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fb3d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3fb3d-124">Accept</span></span>|<span data-ttu-id="3fb3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3fb3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fb3d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fb3d-126">Request body</span></span>
<span data-ttu-id="3fb3d-127">В тексте запроса добавьте представление объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-127">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="3fb3d-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="3fb3d-128">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="3fb3d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fb3d-129">Property</span></span>|<span data-ttu-id="3fb3d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3fb3d-130">Type</span></span>|<span data-ttu-id="3fb3d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3fb3d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fb3d-132">id</span><span class="sxs-lookup"><span data-stu-id="3fb3d-132">id</span></span>|<span data-ttu-id="3fb3d-133">String</span><span class="sxs-lookup"><span data-stu-id="3fb3d-133">String</span></span>|<span data-ttu-id="3fb3d-134">Ключ объекта назначения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-134">Key of the device health script assignment entity.</span></span> <span data-ttu-id="3fb3d-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-135">This property is read-only.</span></span>|
|<span data-ttu-id="3fb3d-136">target</span><span class="sxs-lookup"><span data-stu-id="3fb3d-136">target</span></span>|[<span data-ttu-id="3fb3d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3fb3d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3fb3d-138">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="3fb3d-138">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="3fb3d-139">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="3fb3d-139">runRemediationScript</span></span>|<span data-ttu-id="3fb3d-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fb3d-140">Boolean</span></span>|<span data-ttu-id="3fb3d-141">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-141">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="3fb3d-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="3fb3d-142">runSchedule</span></span>|[<span data-ttu-id="3fb3d-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="3fb3d-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="3fb3d-144">Расписание запуска сценария для целевой группы</span><span class="sxs-lookup"><span data-stu-id="3fb3d-144">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="3fb3d-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fb3d-145">Response</span></span>
<span data-ttu-id="3fb3d-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-146">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fb3d-147">Пример</span><span class="sxs-lookup"><span data-stu-id="3fb3d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fb3d-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fb3d-148">Request</span></span>
<span data-ttu-id="3fb3d-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3fb3d-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fb3d-150">Response</span></span>
<span data-ttu-id="3fb3d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3fb3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





