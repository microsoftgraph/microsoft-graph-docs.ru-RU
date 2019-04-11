---
title: Создание Виндовсаутопилотдеплойментпрофилеассигнмент
description: Создание нового объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aae1abec1a2e3aca42f79a9c133c578c86b16849
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772218"
---
# <a name="create-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="9623c-103">Создание Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="9623c-103">Create windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="9623c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9623c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9623c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9623c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9623c-106">Создание нового объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="9623c-106">Create a new [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9623c-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9623c-107">Prerequisites</span></span>
<span data-ttu-id="9623c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9623c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9623c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9623c-110">Permission type</span></span>|<span data-ttu-id="9623c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9623c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9623c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9623c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9623c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9623c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9623c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9623c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9623c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9623c-115">Not supported.</span></span>|
|<span data-ttu-id="9623c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9623c-116">Application</span></span>|<span data-ttu-id="9623c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9623c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9623c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9623c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9623c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9623c-119">Request headers</span></span>
|<span data-ttu-id="9623c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9623c-120">Header</span></span>|<span data-ttu-id="9623c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9623c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9623c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9623c-122">Authorization</span></span>|<span data-ttu-id="9623c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9623c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9623c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9623c-124">Accept</span></span>|<span data-ttu-id="9623c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9623c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9623c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9623c-126">Request body</span></span>
<span data-ttu-id="9623c-127">В тексте запроса добавьте представление объекта Виндовсаутопилотдеплойментпрофилеассигнмент в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9623c-127">In the request body, supply a JSON representation for the windowsAutopilotDeploymentProfileAssignment object.</span></span>

<span data-ttu-id="9623c-128">В следующей таблице приведены свойства, необходимые при создании Виндовсаутопилотдеплойментпрофилеассигнмент.</span><span class="sxs-lookup"><span data-stu-id="9623c-128">The following table shows the properties that are required when you create the windowsAutopilotDeploymentProfileAssignment.</span></span>

|<span data-ttu-id="9623c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9623c-129">Property</span></span>|<span data-ttu-id="9623c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9623c-130">Type</span></span>|<span data-ttu-id="9623c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9623c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9623c-132">id</span><span class="sxs-lookup"><span data-stu-id="9623c-132">id</span></span>|<span data-ttu-id="9623c-133">String</span><span class="sxs-lookup"><span data-stu-id="9623c-133">String</span></span>|<span data-ttu-id="9623c-134">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="9623c-134">The key of the assignment.</span></span>|
|<span data-ttu-id="9623c-135">target</span><span class="sxs-lookup"><span data-stu-id="9623c-135">target</span></span>|[<span data-ttu-id="9623c-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9623c-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9623c-137">Цель назначения для профиля развертывания Windows для автопилота.</span><span class="sxs-lookup"><span data-stu-id="9623c-137">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="9623c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9623c-138">Response</span></span>
<span data-ttu-id="9623c-139">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9623c-139">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9623c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="9623c-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9623c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="9623c-141">Request</span></span>
<span data-ttu-id="9623c-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9623c-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9623c-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9623c-143">Response</span></span>
<span data-ttu-id="9623c-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9623c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





