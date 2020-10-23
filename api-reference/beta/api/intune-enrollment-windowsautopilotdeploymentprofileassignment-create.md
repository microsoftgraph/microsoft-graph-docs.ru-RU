---
title: Создание Виндовсаутопилотдеплойментпрофилеассигнмент
description: Создание нового объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8055a557b60de674c6d3ce8aad288bfb2e12893
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724215"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="3f332-103">Создание Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="3f332-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

<span data-ttu-id="3f332-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f332-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f332-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f332-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f332-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f332-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f332-107">Создание нового объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="3f332-107">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f332-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3f332-108">Prerequisites</span></span>
<span data-ttu-id="3f332-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f332-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f332-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f332-111">Permission type</span></span>|<span data-ttu-id="3f332-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f332-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f332-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f332-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f332-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f332-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3f332-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f332-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f332-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f332-116">Not supported.</span></span>|
|<span data-ttu-id="3f332-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3f332-117">Application</span></span>|<span data-ttu-id="3f332-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f332-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f332-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f332-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="3f332-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3f332-120">Request headers</span></span>
|<span data-ttu-id="3f332-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f332-121">Header</span></span>|<span data-ttu-id="3f332-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3f332-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f332-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f332-123">Authorization</span></span>|<span data-ttu-id="3f332-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f332-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f332-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f332-125">Accept</span></span>|<span data-ttu-id="3f332-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f332-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f332-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3f332-127">Request body</span></span>
<span data-ttu-id="3f332-128">В тексте запроса добавьте представление объекта Виндовсаутопилотдеплойментпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f332-128">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="3f332-129">В следующей таблице приведены свойства, необходимые при создании Виндовсаутопилотдеплойментпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="3f332-129">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="3f332-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f332-130">Property</span></span>|<span data-ttu-id="3f332-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3f332-131">Type</span></span>|<span data-ttu-id="3f332-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3f332-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f332-133">id</span><span class="sxs-lookup"><span data-stu-id="3f332-133">id</span></span>|<span data-ttu-id="3f332-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3f332-134">String</span></span>|<span data-ttu-id="3f332-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="3f332-135">The key of the assignment.</span></span>|
|<span data-ttu-id="3f332-136">target</span><span class="sxs-lookup"><span data-stu-id="3f332-136">target</span></span>|[<span data-ttu-id="3f332-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3f332-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="3f332-138">Цель назначения для профиля развертывания Windows для автопилота.</span><span class="sxs-lookup"><span data-stu-id="3f332-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|
|<span data-ttu-id="3f332-139">source</span><span class="sxs-lookup"><span data-stu-id="3f332-139">source</span></span>|[<span data-ttu-id="3f332-140">deviceAndAppManagementAssignmentSource</span><span class="sxs-lookup"><span data-stu-id="3f332-140">deviceAndAppManagementAssignmentSource</span></span>](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|<span data-ttu-id="3f332-141">Тип ресурса, используемого для развертывания в группу, Direct или в упаковке/набор политик.</span><span class="sxs-lookup"><span data-stu-id="3f332-141">Type of resource used for deployment to a group, direct or parcel/policySet.</span></span> <span data-ttu-id="3f332-142">Возможные значения: `direct`, `policySets`.</span><span class="sxs-lookup"><span data-stu-id="3f332-142">Possible values are: `direct`, `policySets`.</span></span>|
|<span data-ttu-id="3f332-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="3f332-143">sourceId</span></span>|<span data-ttu-id="3f332-144">Строка</span><span class="sxs-lookup"><span data-stu-id="3f332-144">String</span></span>|<span data-ttu-id="3f332-145">Идентификатор ресурса, используемого для развертывания в группе</span><span class="sxs-lookup"><span data-stu-id="3f332-145">Identifier for resource used for deployment to a group</span></span>|



## <a name="response"></a><span data-ttu-id="3f332-146">Ответ</span><span class="sxs-lookup"><span data-stu-id="3f332-146">Response</span></span>
<span data-ttu-id="3f332-147">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3f332-147">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f332-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3f332-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f332-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f332-149">Request</span></span>
<span data-ttu-id="3f332-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f332-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
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

### <a name="response"></a><span data-ttu-id="3f332-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f332-151">Response</span></span>
<span data-ttu-id="3f332-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3f332-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





