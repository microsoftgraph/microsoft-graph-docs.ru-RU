---
title: Создание Девицехеалсскриптассигнмент
description: Создание нового объекта Девицехеалсскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d0ad1e7ac64b1f849a2e95a427ad41f8571138e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732862"
---
# <a name="create-devicehealthscriptassignment"></a><span data-ttu-id="18dce-103">Создание Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="18dce-103">Create deviceHealthScriptAssignment</span></span>

<span data-ttu-id="18dce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18dce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18dce-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18dce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18dce-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18dce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18dce-107">Создание нового объекта [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="18dce-107">Create a new [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18dce-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="18dce-108">Prerequisites</span></span>
<span data-ttu-id="18dce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18dce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18dce-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18dce-111">Permission type</span></span>|<span data-ttu-id="18dce-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="18dce-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18dce-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18dce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="18dce-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18dce-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="18dce-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18dce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18dce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18dce-116">Not supported.</span></span>|
|<span data-ttu-id="18dce-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18dce-117">Application</span></span>|<span data-ttu-id="18dce-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="18dce-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="18dce-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18dce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="18dce-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="18dce-120">Request headers</span></span>
|<span data-ttu-id="18dce-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18dce-121">Header</span></span>|<span data-ttu-id="18dce-122">Значение</span><span class="sxs-lookup"><span data-stu-id="18dce-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18dce-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18dce-123">Authorization</span></span>|<span data-ttu-id="18dce-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18dce-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18dce-125">Accept</span><span class="sxs-lookup"><span data-stu-id="18dce-125">Accept</span></span>|<span data-ttu-id="18dce-126">application/json</span><span class="sxs-lookup"><span data-stu-id="18dce-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18dce-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="18dce-127">Request body</span></span>
<span data-ttu-id="18dce-128">В тексте запроса добавьте представление объекта Девицехеалсскриптассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18dce-128">In the request body, supply a JSON representation for the deviceHealthScriptAssignment object.</span></span>

<span data-ttu-id="18dce-129">В следующей таблице приведены свойства, необходимые при создании Девицехеалсскриптассигнмент.</span><span class="sxs-lookup"><span data-stu-id="18dce-129">The following table shows the properties that are required when you create the deviceHealthScriptAssignment.</span></span>

|<span data-ttu-id="18dce-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="18dce-130">Property</span></span>|<span data-ttu-id="18dce-131">Тип</span><span class="sxs-lookup"><span data-stu-id="18dce-131">Type</span></span>|<span data-ttu-id="18dce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="18dce-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18dce-133">id</span><span class="sxs-lookup"><span data-stu-id="18dce-133">id</span></span>|<span data-ttu-id="18dce-134">Строка</span><span class="sxs-lookup"><span data-stu-id="18dce-134">String</span></span>|<span data-ttu-id="18dce-135">Ключ объекта назначения сценария работоспособности устройства.</span><span class="sxs-lookup"><span data-stu-id="18dce-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="18dce-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18dce-136">This property is read-only.</span></span>|
|<span data-ttu-id="18dce-137">target</span><span class="sxs-lookup"><span data-stu-id="18dce-137">target</span></span>|[<span data-ttu-id="18dce-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="18dce-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="18dce-139">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="18dce-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="18dce-140">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="18dce-140">runRemediationScript</span></span>|<span data-ttu-id="18dce-141">Логический</span><span class="sxs-lookup"><span data-stu-id="18dce-141">Boolean</span></span>|<span data-ttu-id="18dce-142">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="18dce-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="18dce-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="18dce-143">runSchedule</span></span>|[<span data-ttu-id="18dce-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="18dce-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="18dce-145">Расписание запуска сценария для целевой группы</span><span class="sxs-lookup"><span data-stu-id="18dce-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="18dce-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="18dce-146">Response</span></span>
<span data-ttu-id="18dce-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицехеалсскриптассигнмент](../resources/intune-devices-devicehealthscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18dce-147">If successful, this method returns a `201 Created` response code and a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="18dce-148">Пример</span><span class="sxs-lookup"><span data-stu-id="18dce-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="18dce-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="18dce-149">Request</span></span>
<span data-ttu-id="18dce-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18dce-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments
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

### <a name="response"></a><span data-ttu-id="18dce-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="18dce-151">Response</span></span>
<span data-ttu-id="18dce-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18dce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





