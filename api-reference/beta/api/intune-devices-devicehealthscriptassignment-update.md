---
title: Обновление устройстваHealthScriptAssignment
description: Обновление свойств объекта deviceHealthScriptAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 93909516b037e7545716156920dfec7a089cebca
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610006"
---
# <a name="update-devicehealthscriptassignment"></a><span data-ttu-id="00d58-103">Обновление устройстваHealthScriptAssignment</span><span class="sxs-lookup"><span data-stu-id="00d58-103">Update deviceHealthScriptAssignment</span></span>

<span data-ttu-id="00d58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00d58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00d58-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00d58-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00d58-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00d58-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00d58-107">Обновление свойств объекта [deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="00d58-107">Update the properties of a [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00d58-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00d58-108">Prerequisites</span></span>
<span data-ttu-id="00d58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00d58-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00d58-111">Permission type</span></span>|<span data-ttu-id="00d58-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00d58-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00d58-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00d58-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00d58-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00d58-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00d58-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00d58-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00d58-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00d58-116">Not supported.</span></span>|
|<span data-ttu-id="00d58-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="00d58-117">Application</span></span>|<span data-ttu-id="00d58-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00d58-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00d58-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00d58-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/assignments/{deviceHealthScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="00d58-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00d58-120">Request headers</span></span>
|<span data-ttu-id="00d58-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00d58-121">Header</span></span>|<span data-ttu-id="00d58-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00d58-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00d58-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00d58-123">Authorization</span></span>|<span data-ttu-id="00d58-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00d58-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00d58-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00d58-125">Accept</span></span>|<span data-ttu-id="00d58-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00d58-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00d58-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00d58-127">Request body</span></span>
<span data-ttu-id="00d58-128">В теле запроса поставляем представление JSON для [объекта deviceHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="00d58-128">In the request body, supply a JSON representation for the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object.</span></span>

<span data-ttu-id="00d58-129">В следующей таблице показаны свойства, необходимые при создании [устройстваHealthScriptAssignment.](../resources/intune-devices-devicehealthscriptassignment.md)</span><span class="sxs-lookup"><span data-stu-id="00d58-129">The following table shows the properties that are required when you create the [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md).</span></span>

|<span data-ttu-id="00d58-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00d58-130">Property</span></span>|<span data-ttu-id="00d58-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00d58-131">Type</span></span>|<span data-ttu-id="00d58-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00d58-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00d58-133">id</span><span class="sxs-lookup"><span data-stu-id="00d58-133">id</span></span>|<span data-ttu-id="00d58-134">String</span><span class="sxs-lookup"><span data-stu-id="00d58-134">String</span></span>|<span data-ttu-id="00d58-135">Ключ объекта назначения скрипта для скрипта устройства.</span><span class="sxs-lookup"><span data-stu-id="00d58-135">Key of the device health script assignment entity.</span></span> <span data-ttu-id="00d58-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="00d58-136">This property is read-only.</span></span>|
|<span data-ttu-id="00d58-137">target</span><span class="sxs-lookup"><span data-stu-id="00d58-137">target</span></span>|[<span data-ttu-id="00d58-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="00d58-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="00d58-139">Группа Azure Active Directory, нацелив сценарий на</span><span class="sxs-lookup"><span data-stu-id="00d58-139">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="00d58-140">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="00d58-140">runRemediationScript</span></span>|<span data-ttu-id="00d58-141">Логический</span><span class="sxs-lookup"><span data-stu-id="00d58-141">Boolean</span></span>|<span data-ttu-id="00d58-142">Определите, нужно ли запускать только сценарий обнаружения или запускать сценарий обнаружения и сценарий восстановления.</span><span class="sxs-lookup"><span data-stu-id="00d58-142">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="00d58-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="00d58-143">runSchedule</span></span>|[<span data-ttu-id="00d58-144">deviceHealthScriptRunSchedule</span><span class="sxs-lookup"><span data-stu-id="00d58-144">deviceHealthScriptRunSchedule</span></span>](../resources/intune-devices-devicehealthscriptrunschedule.md)|<span data-ttu-id="00d58-145">Расписание запуска скрипта для целевой группы</span><span class="sxs-lookup"><span data-stu-id="00d58-145">Script run schedule for the target group</span></span>|



## <a name="response"></a><span data-ttu-id="00d58-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="00d58-146">Response</span></span>
<span data-ttu-id="00d58-147">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="00d58-147">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptAssignment](../resources/intune-devices-devicehealthscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00d58-148">Пример</span><span class="sxs-lookup"><span data-stu-id="00d58-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="00d58-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="00d58-149">Request</span></span>
<span data-ttu-id="00d58-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00d58-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/assignments/{deviceHealthScriptAssignmentId}
Content-type: application/json
Content-length: 590

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
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
```

### <a name="response"></a><span data-ttu-id="00d58-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="00d58-151">Response</span></span>
<span data-ttu-id="00d58-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00d58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
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
```




