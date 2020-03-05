---
title: Создание Девицехеалсскриптассигнмент
description: Создание нового объекта Девицехеалсскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: abe35146756d70acb737334e7958f8f77cf9fe24
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469680"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="82f1e-103">Создание Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="82f1e-103">Create deviceHealthScriptAssignment</span></span>

<span data-ttu-id="82f1e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="82f1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82f1e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82f1e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82f1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82f1e-107">Создание нового объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="82f1e-107">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82f1e-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="82f1e-108">Prerequisites</span></span>
<span data-ttu-id="82f1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82f1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82f1e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82f1e-111">Permission type</span></span>|<span data-ttu-id="82f1e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82f1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82f1e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82f1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82f1e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82f1e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="82f1e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82f1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82f1e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82f1e-116">Not supported.</span></span>|
|<span data-ttu-id="82f1e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82f1e-117">Application</span></span>|<span data-ttu-id="82f1e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82f1e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82f1e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82f1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="82f1e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="82f1e-120">Request headers</span></span>
|<span data-ttu-id="82f1e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82f1e-121">Header</span></span>|<span data-ttu-id="82f1e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="82f1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82f1e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="82f1e-123">Authorization</span></span>|<span data-ttu-id="82f1e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82f1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82f1e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82f1e-125">Accept</span></span>|<span data-ttu-id="82f1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82f1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82f1e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82f1e-127">Request body</span></span>
<span data-ttu-id="82f1e-128">В тексте запроса добавьте представление объекта Девицехеалсскриптассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82f1e-128">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="82f1e-129">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскриптассигнмент.</span><span class="sxs-lookup"><span data-stu-id="82f1e-129">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="82f1e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="82f1e-130">Property</span></span>|<span data-ttu-id="82f1e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="82f1e-131">Type</span></span>|<span data-ttu-id="82f1e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="82f1e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82f1e-133">id</span><span class="sxs-lookup"><span data-stu-id="82f1e-133">id</span></span>|<span data-ttu-id="82f1e-134">String</span><span class="sxs-lookup"><span data-stu-id="82f1e-134">String</span></span>|<span data-ttu-id="82f1e-135">Ключ объекта назначения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="82f1e-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="82f1e-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="82f1e-136">This property is read-only.</span></span>|
|<span data-ttu-id="82f1e-137">target</span><span class="sxs-lookup"><span data-stu-id="82f1e-137">target</span></span>|[<span data-ttu-id="82f1e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="82f1e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="82f1e-139">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="82f1e-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="82f1e-140">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="82f1e-140">runRemediationScript</span></span>|<span data-ttu-id="82f1e-141">Логический</span><span class="sxs-lookup"><span data-stu-id="82f1e-141">Boolean</span></span>|<span data-ttu-id="82f1e-142">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="82f1e-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="82f1e-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="82f1e-143">runSchedule</span></span>|[<span data-ttu-id="82f1e-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="82f1e-144">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="82f1e-145">Расписание запуска сценария для целевой группы</span><span class="sxs-lookup"><span data-stu-id="82f1e-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="82f1e-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f1e-146">Response</span></span>
<span data-ttu-id="82f1e-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82f1e-147">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82f1e-148">Пример</span><span class="sxs-lookup"><span data-stu-id="82f1e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="82f1e-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="82f1e-149">Request</span></span>
<span data-ttu-id="82f1e-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82f1e-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82f1e-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="82f1e-151">Response</span></span>
<span data-ttu-id="82f1e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82f1e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





