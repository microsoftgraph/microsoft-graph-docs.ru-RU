---
title: Создание Девицехеалсскриптассигнмент
description: Создание нового объекта Девицехеалсскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e088f2802c68f0d07cc44529e42a70b4f5936ee2
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087603"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="7816e-103">Создание Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="7816e-103">Create deviceHealthScriptAssignment</span></span>

> <span data-ttu-id="7816e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7816e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7816e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7816e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7816e-106">Создание нового объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="7816e-106">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7816e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7816e-107">Prerequisites</span></span>
<span data-ttu-id="7816e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7816e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7816e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7816e-110">Permission type</span></span>|<span data-ttu-id="7816e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7816e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7816e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7816e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7816e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7816e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7816e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7816e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7816e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7816e-115">Not supported.</span></span>|
|<span data-ttu-id="7816e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7816e-116">Application</span></span>|<span data-ttu-id="7816e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7816e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7816e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7816e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7816e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7816e-119">Request headers</span></span>
|<span data-ttu-id="7816e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7816e-120">Header</span></span>|<span data-ttu-id="7816e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7816e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7816e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7816e-122">Authorization</span></span>|<span data-ttu-id="7816e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7816e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7816e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7816e-124">Accept</span></span>|<span data-ttu-id="7816e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7816e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7816e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7816e-126">Request body</span></span>
<span data-ttu-id="7816e-127">В тексте запроса добавьте представление объекта Девицехеалсскриптассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7816e-127">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="7816e-128">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскриптассигнмент.</span><span class="sxs-lookup"><span data-stu-id="7816e-128">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="7816e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7816e-129">Property</span></span>|<span data-ttu-id="7816e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7816e-130">Type</span></span>|<span data-ttu-id="7816e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7816e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7816e-132">id</span><span class="sxs-lookup"><span data-stu-id="7816e-132">id</span></span>|<span data-ttu-id="7816e-133">String</span><span class="sxs-lookup"><span data-stu-id="7816e-133">String</span></span>|<span data-ttu-id="7816e-134">Ключ объекта назначения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="7816e-134">Key of the device health script assignment entity.</span></span> <span data-ttu-id="7816e-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7816e-135">This property is read-only.</span></span>|
|<span data-ttu-id="7816e-136">target</span><span class="sxs-lookup"><span data-stu-id="7816e-136">target</span></span>|[<span data-ttu-id="7816e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7816e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7816e-138">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="7816e-138">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="7816e-139">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="7816e-139">runRemediationScript</span></span>|<span data-ttu-id="7816e-140">Логический</span><span class="sxs-lookup"><span data-stu-id="7816e-140">Boolean</span></span>|<span data-ttu-id="7816e-141">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="7816e-141">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="7816e-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="7816e-142">runSchedule</span></span>|[<span data-ttu-id="7816e-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="7816e-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="7816e-144">Расписание запуска сценария для целевой группы</span><span class="sxs-lookup"><span data-stu-id="7816e-144">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="7816e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="7816e-145">Response</span></span>
<span data-ttu-id="7816e-146">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7816e-146">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7816e-147">Пример</span><span class="sxs-lookup"><span data-stu-id="7816e-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="7816e-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="7816e-148">Request</span></span>
<span data-ttu-id="7816e-149">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7816e-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="7816e-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="7816e-150">Response</span></span>
<span data-ttu-id="7816e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7816e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






