---
title: Создание Девицеманажементскриптассигнмент
description: Создание нового объекта Девицеманажементскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c01b55570dfb7886c4935d40dc9c56e69a1f67d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469491"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="d8b67-103">Создание Девицеманажементскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="d8b67-103">Create deviceManagementScriptAssignment</span></span>

<span data-ttu-id="d8b67-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d8b67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8b67-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8b67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8b67-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8b67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8b67-107">Создание нового объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="d8b67-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8b67-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d8b67-108">Prerequisites</span></span>
<span data-ttu-id="d8b67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8b67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8b67-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8b67-111">Permission type</span></span>|<span data-ttu-id="d8b67-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8b67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8b67-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8b67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8b67-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b67-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d8b67-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8b67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8b67-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8b67-116">Not supported.</span></span>|
|<span data-ttu-id="d8b67-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8b67-117">Application</span></span>|<span data-ttu-id="d8b67-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8b67-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8b67-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8b67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="d8b67-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8b67-120">Request headers</span></span>
|<span data-ttu-id="d8b67-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8b67-121">Header</span></span>|<span data-ttu-id="d8b67-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d8b67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8b67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8b67-123">Authorization</span></span>|<span data-ttu-id="d8b67-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8b67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8b67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d8b67-125">Accept</span></span>|<span data-ttu-id="d8b67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8b67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8b67-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8b67-127">Request body</span></span>
<span data-ttu-id="d8b67-128">В тексте запроса добавьте представление объекта Девицеманажементскриптассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8b67-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="d8b67-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптассигнмент.</span><span class="sxs-lookup"><span data-stu-id="d8b67-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="d8b67-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8b67-130">Property</span></span>|<span data-ttu-id="d8b67-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d8b67-131">Type</span></span>|<span data-ttu-id="d8b67-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d8b67-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8b67-133">id</span><span class="sxs-lookup"><span data-stu-id="d8b67-133">id</span></span>|<span data-ttu-id="d8b67-134">String</span><span class="sxs-lookup"><span data-stu-id="d8b67-134">String</span></span>|<span data-ttu-id="d8b67-135">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="d8b67-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="d8b67-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d8b67-136">This property is read-only.</span></span>|
|<span data-ttu-id="d8b67-137">target</span><span class="sxs-lookup"><span data-stu-id="d8b67-137">target</span></span>|[<span data-ttu-id="d8b67-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d8b67-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d8b67-139">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="d8b67-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="d8b67-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8b67-140">Response</span></span>
<span data-ttu-id="d8b67-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8b67-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8b67-142">Пример</span><span class="sxs-lookup"><span data-stu-id="d8b67-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8b67-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8b67-143">Request</span></span>
<span data-ttu-id="d8b67-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8b67-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="d8b67-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8b67-145">Response</span></span>
<span data-ttu-id="d8b67-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8b67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "a87a601e-601e-a87a-1e60-7aa81e607aa8",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





