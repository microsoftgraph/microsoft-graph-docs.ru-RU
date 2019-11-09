---
title: Обновление Девицеманажементскриптассигнмент
description: Обновление свойств объекта Девицеманажементскриптассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c786deeaab6e5ebef156b1171800ebdb7da2e872
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087540"
---
# <a name="update-devicemanagementscriptassignment"></a><span data-ttu-id="562c1-103">Обновление Девицеманажементскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="562c1-103">Update deviceManagementScriptAssignment</span></span>

> <span data-ttu-id="562c1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="562c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="562c1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="562c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="562c1-106">Обновление свойств объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="562c1-106">Update the properties of a [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="562c1-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="562c1-107">Prerequisites</span></span>
<span data-ttu-id="562c1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="562c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="562c1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="562c1-110">Permission type</span></span>|<span data-ttu-id="562c1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="562c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="562c1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="562c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="562c1-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="562c1-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="562c1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="562c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="562c1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="562c1-115">Not supported.</span></span>|
|<span data-ttu-id="562c1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="562c1-116">Application</span></span>|<span data-ttu-id="562c1-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="562c1-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="562c1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="562c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="562c1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="562c1-119">Request headers</span></span>
|<span data-ttu-id="562c1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="562c1-120">Header</span></span>|<span data-ttu-id="562c1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="562c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="562c1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="562c1-122">Authorization</span></span>|<span data-ttu-id="562c1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="562c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="562c1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="562c1-124">Accept</span></span>|<span data-ttu-id="562c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="562c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="562c1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="562c1-126">Request body</span></span>
<span data-ttu-id="562c1-127">В тексте запроса добавьте представление объекта [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="562c1-127">In the request body, supply a JSON representation for the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object.</span></span>

<span data-ttu-id="562c1-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md).</span><span class="sxs-lookup"><span data-stu-id="562c1-128">The following table shows the properties that are required when you create the [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).</span></span>

|<span data-ttu-id="562c1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="562c1-129">Property</span></span>|<span data-ttu-id="562c1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="562c1-130">Type</span></span>|<span data-ttu-id="562c1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="562c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="562c1-132">id</span><span class="sxs-lookup"><span data-stu-id="562c1-132">id</span></span>|<span data-ttu-id="562c1-133">String</span><span class="sxs-lookup"><span data-stu-id="562c1-133">String</span></span>|<span data-ttu-id="562c1-134">Ключ объекта назначения группы сценариев управления устройствами.</span><span class="sxs-lookup"><span data-stu-id="562c1-134">Key of the device management script group assignment entity.</span></span> <span data-ttu-id="562c1-135">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="562c1-135">This property is read-only.</span></span>|
|<span data-ttu-id="562c1-136">target</span><span class="sxs-lookup"><span data-stu-id="562c1-136">target</span></span>|[<span data-ttu-id="562c1-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="562c1-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="562c1-138">Идентификатор группы Azure Active Directory, на которую ориентирован сценарий.</span><span class="sxs-lookup"><span data-stu-id="562c1-138">The Id of the Azure Active Directory group we are targeting the script to.</span></span>|



## <a name="response"></a><span data-ttu-id="562c1-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="562c1-139">Response</span></span>
<span data-ttu-id="562c1-140">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементскриптассигнмент](../resources/intune-devices-devicemanagementscriptassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="562c1-140">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="562c1-141">Пример</span><span class="sxs-lookup"><span data-stu-id="562c1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="562c1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="562c1-142">Request</span></span>
<span data-ttu-id="562c1-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="562c1-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/assignments/{deviceManagementScriptAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="562c1-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="562c1-144">Response</span></span>
<span data-ttu-id="562c1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="562c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






