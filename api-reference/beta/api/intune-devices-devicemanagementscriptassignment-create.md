---
title: Создание Девицеманажементскриптассигнмент
description: Создание нового объекта Девицеманажементскриптассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1557b1eb4408ebfe9200d5cf83cb9e5fe55259e9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43426202"
---
# <a name="create-devicemanagementscriptassignment"></a><span data-ttu-id="1ed19-103">Создание Девицеманажементскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="1ed19-103">Create deviceManagementScriptAssignment</span></span>

<span data-ttu-id="1ed19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ed19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ed19-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed19-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed19-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ed19-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed19-107">Создание нового объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1ed19-107">Create a new [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ed19-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1ed19-108">Prerequisites</span></span>
<span data-ttu-id="1ed19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ed19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ed19-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ed19-111">Permission type</span></span>|<span data-ttu-id="1ed19-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ed19-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ed19-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ed19-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ed19-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed19-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1ed19-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ed19-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ed19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ed19-116">Not supported.</span></span>|
|<span data-ttu-id="1ed19-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1ed19-117">Application</span></span>|<span data-ttu-id="1ed19-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ed19-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ed19-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ed19-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts/{deviceShellScriptId}/assignments
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1ed19-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1ed19-120">Request headers</span></span>
|<span data-ttu-id="1ed19-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1ed19-121">Header</span></span>|<span data-ttu-id="1ed19-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1ed19-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ed19-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ed19-123">Authorization</span></span>|<span data-ttu-id="1ed19-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ed19-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ed19-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ed19-125">Accept</span></span>|<span data-ttu-id="1ed19-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ed19-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ed19-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ed19-127">Request body</span></span>
<span data-ttu-id="1ed19-128">В тексте запроса добавьте представление объекта Девицеманажементскриптассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ed19-128">In the request body, supply a JSON representation for the deviceManagementScriptAssignment object.</span></span>

<span data-ttu-id="1ed19-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементскриптассигнмент.</span><span class="sxs-lookup"><span data-stu-id="1ed19-129">The following table shows the properties that are required when you create the deviceManagementScriptAssignment.</span></span>

|<span data-ttu-id="1ed19-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ed19-130">Property</span></span>|<span data-ttu-id="1ed19-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1ed19-131">Type</span></span>|<span data-ttu-id="1ed19-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1ed19-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed19-133">id</span><span class="sxs-lookup"><span data-stu-id="1ed19-133">id</span></span>|<span data-ttu-id="1ed19-134">String</span><span class="sxs-lookup"><span data-stu-id="1ed19-134">String</span></span>|<span data-ttu-id="1ed19-135">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="1ed19-135">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="1ed19-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1ed19-136">This property is read-only.</span></span>|
|<span data-ttu-id="1ed19-137">target</span><span class="sxs-lookup"><span data-stu-id="1ed19-137">target</span></span>|[<span data-ttu-id="1ed19-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1ed19-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1ed19-139">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="1ed19-139">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="1ed19-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ed19-140">Response</span></span>
<span data-ttu-id="1ed19-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1ed19-141">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ed19-142">Пример</span><span class="sxs-lookup"><span data-stu-id="1ed19-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ed19-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ed19-143">Request</span></span>
<span data-ttu-id="1ed19-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ed19-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ed19-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ed19-145">Response</span></span>
<span data-ttu-id="1ed19-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1ed19-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



