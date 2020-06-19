---
title: Обновление Виндовсаутопилотдеплойментпрофилеассигнмент
description: Обновление свойств объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 168616aa23934d5aa5e01d995cda533ed7d786e4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792038"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="187fc-103">Обновление Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="187fc-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="187fc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="187fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="187fc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="187fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="187fc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="187fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="187fc-107">Обновление свойств объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="187fc-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="187fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="187fc-108">Prerequisites</span></span>
<span data-ttu-id="187fc-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="187fc-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="187fc-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="187fc-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="187fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="187fc-111">Permission type</span></span>|<span data-ttu-id="187fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="187fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="187fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="187fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="187fc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="187fc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="187fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="187fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="187fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="187fc-116">Not supported.</span></span>|
|<span data-ttu-id="187fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="187fc-117">Application</span></span>|<span data-ttu-id="187fc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="187fc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="187fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="187fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="187fc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="187fc-120">Request headers</span></span>
|<span data-ttu-id="187fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="187fc-121">Header</span></span>|<span data-ttu-id="187fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="187fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="187fc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="187fc-123">Authorization</span></span>|<span data-ttu-id="187fc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="187fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="187fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="187fc-125">Accept</span></span>|<span data-ttu-id="187fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="187fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="187fc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="187fc-127">Request body</span></span>
<span data-ttu-id="187fc-128">В тексте запроса добавьте представление объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="187fc-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="187fc-129">В следующей таблице приведены свойства, необходимые при создании [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="187fc-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="187fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="187fc-130">Property</span></span>|<span data-ttu-id="187fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="187fc-131">Type</span></span>|<span data-ttu-id="187fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="187fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="187fc-133">id</span><span class="sxs-lookup"><span data-stu-id="187fc-133">id</span></span>|<span data-ttu-id="187fc-134">String</span><span class="sxs-lookup"><span data-stu-id="187fc-134">String</span></span>|<span data-ttu-id="187fc-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="187fc-135">The key of the assignment.</span></span>|
|<span data-ttu-id="187fc-136">target</span><span class="sxs-lookup"><span data-stu-id="187fc-136">target</span></span>|[<span data-ttu-id="187fc-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="187fc-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="187fc-138">Цель назначения для профиля развертывания Windows для автопилота.</span><span class="sxs-lookup"><span data-stu-id="187fc-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="187fc-139">source</span><span class="sxs-lookup"><span data-stu-id="187fc-139">source</span></span>|[<span data-ttu-id="187fc-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="187fc-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="187fc-141">Тип ресурса, используемого для развертывания в группу, Direct или в упаковке/набор политик.</span><span class="sxs-lookup"><span data-stu-id="187fc-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="187fc-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="187fc-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="187fc-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="187fc-143">sourceId</span></span>|<span data-ttu-id="187fc-144">String</span><span class="sxs-lookup"><span data-stu-id="187fc-144">String</span></span>|<span data-ttu-id="187fc-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="187fc-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="187fc-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="187fc-146">Response</span></span>
<span data-ttu-id="187fc-147">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="187fc-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="187fc-148">Пример</span><span class="sxs-lookup"><span data-stu-id="187fc-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="187fc-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="187fc-149">Request</span></span>
<span data-ttu-id="187fc-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="187fc-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 411

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```

### <a name="response"></a><span data-ttu-id="187fc-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="187fc-151">Response</span></span>
<span data-ttu-id="187fc-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="187fc-152">Here is an example of the response.</span></span> <span data-ttu-id="187fc-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="187fc-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="187fc-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="187fc-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "source": "policySets",
  "sourceId": "Source Id value"
}
```



