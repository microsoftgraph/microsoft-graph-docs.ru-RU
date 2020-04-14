---
title: Обновление Виндовсаутопилотдеплойментпрофилеассигнмент
description: Обновление свойств объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bb2c3e61569d5d55be55f737ab505ba240c73a87
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452463"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="55c94-103">Обновление Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="55c94-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="55c94-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55c94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55c94-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55c94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55c94-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55c94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55c94-107">Обновление свойств объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="55c94-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55c94-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="55c94-108">Prerequisites</span></span>
<span data-ttu-id="55c94-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55c94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55c94-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="55c94-111">Permission type</span></span>|<span data-ttu-id="55c94-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="55c94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55c94-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="55c94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55c94-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55c94-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="55c94-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="55c94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55c94-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55c94-116">Not supported.</span></span>|
|<span data-ttu-id="55c94-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="55c94-117">Application</span></span>|<span data-ttu-id="55c94-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55c94-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55c94-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="55c94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="55c94-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="55c94-120">Request headers</span></span>
|<span data-ttu-id="55c94-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="55c94-121">Header</span></span>|<span data-ttu-id="55c94-122">Значение</span><span class="sxs-lookup"><span data-stu-id="55c94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55c94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55c94-123">Authorization</span></span>|<span data-ttu-id="55c94-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="55c94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55c94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55c94-125">Accept</span></span>|<span data-ttu-id="55c94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55c94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55c94-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="55c94-127">Request body</span></span>
<span data-ttu-id="55c94-128">В тексте запроса добавьте представление объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55c94-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="55c94-129">В следующей таблице приведены свойства, необходимые при создании [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="55c94-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="55c94-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="55c94-130">Property</span></span>|<span data-ttu-id="55c94-131">Тип</span><span class="sxs-lookup"><span data-stu-id="55c94-131">Type</span></span>|<span data-ttu-id="55c94-132">Описание</span><span class="sxs-lookup"><span data-stu-id="55c94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55c94-133">id</span><span class="sxs-lookup"><span data-stu-id="55c94-133">id</span></span>|<span data-ttu-id="55c94-134">String</span><span class="sxs-lookup"><span data-stu-id="55c94-134">String</span></span>|<span data-ttu-id="55c94-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="55c94-135">The key of the assignment.</span></span>|
|<span data-ttu-id="55c94-136">target</span><span class="sxs-lookup"><span data-stu-id="55c94-136">target</span></span>|[<span data-ttu-id="55c94-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="55c94-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="55c94-138">Цель назначения для профиля развертывания Windows для автопилота.</span><span class="sxs-lookup"><span data-stu-id="55c94-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="55c94-139">source</span><span class="sxs-lookup"><span data-stu-id="55c94-139">source</span></span>|[<span data-ttu-id="55c94-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="55c94-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="55c94-141">Тип ресурса, используемого для развертывания в группу, Direct или в упаковке/набор политик.</span><span class="sxs-lookup"><span data-stu-id="55c94-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="55c94-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="55c94-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="55c94-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="55c94-143">sourceId</span></span>|<span data-ttu-id="55c94-144">String</span><span class="sxs-lookup"><span data-stu-id="55c94-144">String</span></span>|<span data-ttu-id="55c94-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="55c94-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="55c94-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="55c94-146">Response</span></span>
<span data-ttu-id="55c94-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="55c94-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55c94-148">Пример</span><span class="sxs-lookup"><span data-stu-id="55c94-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="55c94-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="55c94-149">Request</span></span>
<span data-ttu-id="55c94-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="55c94-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="55c94-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="55c94-151">Response</span></span>
<span data-ttu-id="55c94-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="55c94-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



