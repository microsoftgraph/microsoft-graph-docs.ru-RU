---
title: Обновление windowsAutopilotDeploymentProfileAssignment
description: Обновление свойств объекта windowsAutopilotDeploymentProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a29522f9d6141be5e2513e9a39f985c53de3306
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142193"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="0391d-103">Обновление windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="0391d-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="0391d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0391d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0391d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0391d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0391d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0391d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0391d-107">Обновление свойств объекта [windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0391d-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0391d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0391d-108">Prerequisites</span></span>
<span data-ttu-id="0391d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0391d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0391d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0391d-111">Permission type</span></span>|<span data-ttu-id="0391d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0391d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0391d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0391d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0391d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0391d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0391d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0391d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0391d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0391d-116">Not supported.</span></span>|
|<span data-ttu-id="0391d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="0391d-117">Application</span></span>|<span data-ttu-id="0391d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0391d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0391d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0391d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="0391d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="0391d-120">Request headers</span></span>
|<span data-ttu-id="0391d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0391d-121">Header</span></span>|<span data-ttu-id="0391d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0391d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0391d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0391d-123">Authorization</span></span>|<span data-ttu-id="0391d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0391d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0391d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0391d-125">Accept</span></span>|<span data-ttu-id="0391d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0391d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0391d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0391d-127">Request body</span></span>
<span data-ttu-id="0391d-128">В теле запроса поставляем представление JSON для [объекта windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0391d-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="0391d-129">В следующей таблице показаны свойства, необходимые при создании [windowsAutopilotDeploymentProfileAssignment.](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0391d-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="0391d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0391d-130">Property</span></span>|<span data-ttu-id="0391d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0391d-131">Type</span></span>|<span data-ttu-id="0391d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0391d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0391d-133">id</span><span class="sxs-lookup"><span data-stu-id="0391d-133">id</span></span>|<span data-ttu-id="0391d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0391d-134">String</span></span>|<span data-ttu-id="0391d-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="0391d-135">The key of the assignment.</span></span>|
|<span data-ttu-id="0391d-136">target</span><span class="sxs-lookup"><span data-stu-id="0391d-136">target</span></span>|[<span data-ttu-id="0391d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0391d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0391d-138">Цель назначения для профиля развертывания автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="0391d-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="0391d-139">source</span><span class="sxs-lookup"><span data-stu-id="0391d-139">source</span></span>|[<span data-ttu-id="0391d-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="0391d-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="0391d-141">Тип ресурса, используемого для развертывания в группу, прямую или пакетную группу/policySet.</span><span class="sxs-lookup"><span data-stu-id="0391d-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="0391d-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="0391d-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="0391d-143">sourceId</span><span class="sxs-lookup"><span data-stu-id="0391d-143">sourceId</span></span>|<span data-ttu-id="0391d-144">Строка</span><span class="sxs-lookup"><span data-stu-id="0391d-144">String</span></span>|<span data-ttu-id="0391d-145">Идентификатор ресурса, используемой для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="0391d-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="0391d-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="0391d-146">Response</span></span>
<span data-ttu-id="0391d-147">В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="0391d-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0391d-148">Пример</span><span class="sxs-lookup"><span data-stu-id="0391d-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="0391d-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="0391d-149">Request</span></span>
<span data-ttu-id="0391d-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0391d-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0391d-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="0391d-151">Response</span></span>
<span data-ttu-id="0391d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0391d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




