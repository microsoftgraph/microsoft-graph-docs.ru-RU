---
title: Обновление Виндовсаутопилотдеплойментпрофилеассигнмент
description: Обновление свойств объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d42a28e0bb6326bcae331eda2c227eca5c62e2c4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187718"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="2d78c-103">Обновление Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="2d78c-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="2d78c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d78c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d78c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2d78c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d78c-106">Обновление свойств объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="2d78c-106">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d78c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2d78c-107">Prerequisites</span></span>
<span data-ttu-id="2d78c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d78c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d78c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d78c-110">Permission type</span></span>|<span data-ttu-id="2d78c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d78c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d78c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d78c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d78c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d78c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d78c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d78c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d78c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d78c-115">Not supported.</span></span>|
|<span data-ttu-id="2d78c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d78c-116">Application</span></span>|<span data-ttu-id="2d78c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d78c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d78c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d78c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="2d78c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d78c-119">Request headers</span></span>
|<span data-ttu-id="2d78c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2d78c-120">Header</span></span>|<span data-ttu-id="2d78c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2d78c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d78c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2d78c-122">Authorization</span></span>|<span data-ttu-id="2d78c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d78c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d78c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2d78c-124">Accept</span></span>|<span data-ttu-id="2d78c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d78c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d78c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2d78c-126">Request body</span></span>
<span data-ttu-id="2d78c-127">В тексте запроса добавьте представление объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d78c-127">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="2d78c-128">В следующей таблице приведены свойства, необходимые при создании [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2d78c-128">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="2d78c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d78c-129">Property</span></span>|<span data-ttu-id="2d78c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2d78c-130">Type</span></span>|<span data-ttu-id="2d78c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2d78c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d78c-132">id</span><span class="sxs-lookup"><span data-stu-id="2d78c-132">id</span></span>|<span data-ttu-id="2d78c-133">String</span><span class="sxs-lookup"><span data-stu-id="2d78c-133">String</span></span>|<span data-ttu-id="2d78c-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="2d78c-134">The key of the assignment.</span></span>|
|<span data-ttu-id="2d78c-135">target</span><span class="sxs-lookup"><span data-stu-id="2d78c-135">target</span></span>|[<span data-ttu-id="2d78c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2d78c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2d78c-137">Цель назначения для профиля развертывания Windows для автопилота.</span><span class="sxs-lookup"><span data-stu-id="2d78c-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="2d78c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d78c-138">Response</span></span>
<span data-ttu-id="2d78c-139">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d78c-139">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d78c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="2d78c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d78c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d78c-141">Request</span></span>
<span data-ttu-id="2d78c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d78c-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="2d78c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d78c-143">Response</span></span>
<span data-ttu-id="2d78c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2d78c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




