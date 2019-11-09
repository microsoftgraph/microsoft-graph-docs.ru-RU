---
title: Обновление Девицехеалсскриптассигнмент
description: Обновление свойств объекта Девицехеалсскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3193e611318c6abf2cff4bbd7c133939d2ee6cae
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087575"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="24046-103">Обновление Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="24046-103">Update deviceHealthScriptAssignment</span></span>

> <span data-ttu-id="24046-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24046-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24046-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24046-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24046-106">Обновление свойств объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="24046-106">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24046-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="24046-107">Prerequisites</span></span>
<span data-ttu-id="24046-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24046-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24046-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="24046-110">Permission type</span></span>|<span data-ttu-id="24046-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="24046-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24046-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="24046-112">Delegated (work or school account)</span></span>|<span data-ttu-id="24046-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24046-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24046-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="24046-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24046-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24046-115">Not supported.</span></span>|
|<span data-ttu-id="24046-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="24046-116">Application</span></span>|<span data-ttu-id="24046-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24046-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24046-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="24046-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="24046-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="24046-119">Request headers</span></span>
|<span data-ttu-id="24046-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="24046-120">Header</span></span>|<span data-ttu-id="24046-121">Значение</span><span class="sxs-lookup"><span data-stu-id="24046-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24046-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="24046-122">Authorization</span></span>|<span data-ttu-id="24046-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="24046-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24046-124">Accept</span><span class="sxs-lookup"><span data-stu-id="24046-124">Accept</span></span>|<span data-ttu-id="24046-125">application/json</span><span class="sxs-lookup"><span data-stu-id="24046-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24046-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="24046-126">Request body</span></span>
<span data-ttu-id="24046-127">В тексте запроса добавьте представление объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24046-127">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="24046-128">В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="24046-128">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="24046-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="24046-129">Property</span></span>|<span data-ttu-id="24046-130">Тип</span><span class="sxs-lookup"><span data-stu-id="24046-130">Type</span></span>|<span data-ttu-id="24046-131">Описание</span><span class="sxs-lookup"><span data-stu-id="24046-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24046-132">id</span><span class="sxs-lookup"><span data-stu-id="24046-132">id</span></span>|<span data-ttu-id="24046-133">String</span><span class="sxs-lookup"><span data-stu-id="24046-133">String</span></span>|<span data-ttu-id="24046-134">Ключ объекта назначения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="24046-134">Key of the device health script assignment entity.</span></span> <span data-ttu-id="24046-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24046-135">This property is read-only.</span></span>|
|<span data-ttu-id="24046-136">target</span><span class="sxs-lookup"><span data-stu-id="24046-136">target</span></span>|[<span data-ttu-id="24046-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="24046-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="24046-138">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="24046-138">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="24046-139">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="24046-139">runRemediationScript</span></span>|<span data-ttu-id="24046-140">Логический</span><span class="sxs-lookup"><span data-stu-id="24046-140">Boolean</span></span>|<span data-ttu-id="24046-141">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="24046-141">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="24046-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="24046-142">runSchedule</span></span>|[<span data-ttu-id="24046-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="24046-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="24046-144">Расписание запуска сценария для целевой группы</span><span class="sxs-lookup"><span data-stu-id="24046-144">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="24046-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="24046-145">Response</span></span>
<span data-ttu-id="24046-146">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="24046-146">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24046-147">Пример</span><span class="sxs-lookup"><span data-stu-id="24046-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="24046-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="24046-148">Request</span></span>
<span data-ttu-id="24046-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="24046-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24046-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="24046-150">Response</span></span>
<span data-ttu-id="24046-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="24046-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






