---
title: Обновление windowsAutopilotDeploymentProfileAssignment
description: Обновление свойства объекта windowsAutopilotDeploymentProfileAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c5ee35e308b5a7392c3dff2c4ead307d9735e0b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837576"
---
# <a name="update-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="94d70-103">Обновление windowsAutopilotDeploymentProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="94d70-103">Update windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="94d70-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94d70-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94d70-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94d70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94d70-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="94d70-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94d70-107">Обновление свойства объекта [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="94d70-107">Update the properties of a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94d70-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="94d70-108">Prerequisites</span></span>
<span data-ttu-id="94d70-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94d70-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94d70-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94d70-111">Permission type</span></span>|<span data-ttu-id="94d70-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="94d70-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94d70-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94d70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="94d70-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94d70-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94d70-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94d70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94d70-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94d70-116">Not supported.</span></span>|
|<span data-ttu-id="94d70-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94d70-117">Application</span></span>|<span data-ttu-id="94d70-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94d70-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94d70-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94d70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="94d70-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94d70-120">Request headers</span></span>
|<span data-ttu-id="94d70-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94d70-121">Header</span></span>|<span data-ttu-id="94d70-122">Значение</span><span class="sxs-lookup"><span data-stu-id="94d70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94d70-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94d70-123">Authorization</span></span>|<span data-ttu-id="94d70-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="94d70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94d70-125">Accept</span><span class="sxs-lookup"><span data-stu-id="94d70-125">Accept</span></span>|<span data-ttu-id="94d70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="94d70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94d70-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="94d70-127">Request body</span></span>
<span data-ttu-id="94d70-128">В тексте запроса укажите представление JSON для объекта [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="94d70-128">In the request body, supply a JSON representation for the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

<span data-ttu-id="94d70-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="94d70-129">The following table shows the properties that are required when you create the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

|<span data-ttu-id="94d70-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="94d70-130">Property</span></span>|<span data-ttu-id="94d70-131">Тип</span><span class="sxs-lookup"><span data-stu-id="94d70-131">Type</span></span>|<span data-ttu-id="94d70-132">Описание</span><span class="sxs-lookup"><span data-stu-id="94d70-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94d70-133">id</span><span class="sxs-lookup"><span data-stu-id="94d70-133">id</span></span>|<span data-ttu-id="94d70-134">String</span><span class="sxs-lookup"><span data-stu-id="94d70-134">String</span></span>|<span data-ttu-id="94d70-135">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="94d70-135">The key of the assignment.</span></span>|
|<span data-ttu-id="94d70-136">target</span><span class="sxs-lookup"><span data-stu-id="94d70-136">target</span></span>|[<span data-ttu-id="94d70-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="94d70-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="94d70-138">Целевой объект назначения для профиля развертывания автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="94d70-138">The assignment target for the Windows Autopilot deployment profile.</span></span>|



## <a name="response"></a><span data-ttu-id="94d70-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="94d70-139">Response</span></span>
<span data-ttu-id="94d70-140">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="94d70-140">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94d70-141">Пример</span><span class="sxs-lookup"><span data-stu-id="94d70-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="94d70-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="94d70-142">Request</span></span>
<span data-ttu-id="94d70-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94d70-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="94d70-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="94d70-144">Response</span></span>
<span data-ttu-id="94d70-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="94d70-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





