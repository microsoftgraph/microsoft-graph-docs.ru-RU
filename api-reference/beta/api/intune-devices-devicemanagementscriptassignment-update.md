---
title: Обновление Девицеманажементскриптассигнмент
description: Обновление свойств объекта Девицеманажементскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 87ea086446a7d5a6db0eec76e28ff9b63fc3e22e
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792347"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="adbc8-103">Обновление Девицеманажементскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="adbc8-103">Update deviceManagementScriptAssignment</span></span>

<span data-ttu-id="adbc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adbc8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adbc8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbc8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adbc8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adbc8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adbc8-107">Обновление свойств объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="adbc8-107">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adbc8-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="adbc8-108">Prerequisites</span></span>
<span data-ttu-id="adbc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="adbc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adbc8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="adbc8-111">Permission type</span></span>|<span data-ttu-id="adbc8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="adbc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adbc8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="adbc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="adbc8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbc8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="adbc8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="adbc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adbc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adbc8-116">Not supported.</span></span>|
|<span data-ttu-id="adbc8-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="adbc8-117">Application</span></span>|<span data-ttu-id="adbc8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adbc8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adbc8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="adbc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="adbc8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="adbc8-120">Request headers</span></span>
|<span data-ttu-id="adbc8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="adbc8-121">Header</span></span>|<span data-ttu-id="adbc8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="adbc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adbc8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="adbc8-123">Authorization</span></span>|<span data-ttu-id="adbc8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="adbc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adbc8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="adbc8-125">Accept</span></span>|<span data-ttu-id="adbc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="adbc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adbc8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="adbc8-127">Request body</span></span>
<span data-ttu-id="adbc8-128">В тексте запроса добавьте представление объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adbc8-128">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="adbc8-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="adbc8-129">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="adbc8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="adbc8-130">Property</span></span>|<span data-ttu-id="adbc8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="adbc8-131">Type</span></span>|<span data-ttu-id="adbc8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="adbc8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adbc8-133">id</span><span class="sxs-lookup"><span data-stu-id="adbc8-133">id</span></span>|<span data-ttu-id="adbc8-134">String</span><span class="sxs-lookup"><span data-stu-id="adbc8-134">String</span></span>|<span data-ttu-id="adbc8-135">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="adbc8-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="adbc8-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="adbc8-136">This property is read-only.</span></span>|
|<span data-ttu-id="adbc8-137">target</span><span class="sxs-lookup"><span data-stu-id="adbc8-137">target</span></span>|[<span data-ttu-id="adbc8-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="adbc8-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="adbc8-139">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="adbc8-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="adbc8-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbc8-140">Response</span></span>
<span data-ttu-id="adbc8-141">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="adbc8-141">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adbc8-142">Пример</span><span class="sxs-lookup"><span data-stu-id="adbc8-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="adbc8-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="adbc8-143">Request</span></span>
<span data-ttu-id="adbc8-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="adbc8-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 327

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a><span data-ttu-id="adbc8-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="adbc8-145">Response</span></span>
<span data-ttu-id="adbc8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="adbc8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```



