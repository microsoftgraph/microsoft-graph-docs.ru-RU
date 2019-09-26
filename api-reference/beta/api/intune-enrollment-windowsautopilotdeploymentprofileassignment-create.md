---
title: Создание Виндовсаутопилотдеплойментпрофилеассигнмент
description: Создание нового объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bff01991a56b5a4fd6c63f591fb973c430987e98
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37187739"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="e0017-103">Создание Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="e0017-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="e0017-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0017-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0017-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0017-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0017-106">Создание нового объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e0017-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0017-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e0017-107">Prerequisites</span></span>
<span data-ttu-id="e0017-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0017-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0017-110">Permission type</span></span>|<span data-ttu-id="e0017-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0017-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0017-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0017-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0017-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0017-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e0017-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0017-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0017-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0017-115">Not supported.</span></span>|
|<span data-ttu-id="e0017-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0017-116">Application</span></span>|<span data-ttu-id="e0017-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0017-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0017-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0017-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e0017-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0017-119">Request headers</span></span>
|<span data-ttu-id="e0017-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0017-120">Header</span></span>|<span data-ttu-id="e0017-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e0017-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0017-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0017-122">Authorization</span></span>|<span data-ttu-id="e0017-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0017-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0017-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e0017-124">Accept</span></span>|<span data-ttu-id="e0017-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0017-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0017-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0017-126">Request body</span></span>
<span data-ttu-id="e0017-127">В тексте запроса добавьте представление объекта Виндовсаутопилотдеплойментпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0017-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="e0017-128">В следующей таблице приведены свойства, необходимые при создании Виндовсаутопилотдеплойментпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="e0017-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="e0017-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0017-129">Property</span></span>|<span data-ttu-id="e0017-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e0017-130">Type</span></span>|<span data-ttu-id="e0017-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e0017-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0017-132">id</span><span class="sxs-lookup"><span data-stu-id="e0017-132">id</span></span>|<span data-ttu-id="e0017-133">String</span><span class="sxs-lookup"><span data-stu-id="e0017-133">String</span></span>|<span data-ttu-id="e0017-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="e0017-134">The key of the assignment.</span></span>|
|<span data-ttu-id="e0017-135">target</span><span class="sxs-lookup"><span data-stu-id="e0017-135">target</span></span>|[<span data-ttu-id="e0017-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e0017-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e0017-137">Цель назначения для профиля развертывания Windows для автопилота.</span><span class="sxs-lookup"><span data-stu-id="e0017-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="e0017-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0017-138">Response</span></span>
<span data-ttu-id="e0017-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e0017-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0017-140">Пример</span><span class="sxs-lookup"><span data-stu-id="e0017-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0017-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0017-141">Request</span></span>
<span data-ttu-id="e0017-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0017-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e0017-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0017-143">Response</span></span>
<span data-ttu-id="e0017-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0017-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




