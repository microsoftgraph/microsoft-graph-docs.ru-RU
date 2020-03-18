---
title: Удаление Виндовсаутопилотдеплойментпрофилеассигнмент
description: Удаляет объект Виндовсаутопилотдеплойментпрофилеассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7cf950b2de93d5f87a79c9fa035f0499e368af99
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805075"
---
# <a name="delete-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="054fa-103">Удаление Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="054fa-103">Delete windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="054fa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="054fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="054fa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="054fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="054fa-106">Удаляет объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span><span class="sxs-lookup"><span data-stu-id="054fa-106">Deletes a [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="054fa-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="054fa-107">Prerequisites</span></span>
<span data-ttu-id="054fa-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="054fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="054fa-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="054fa-110">Permission type</span></span>|<span data-ttu-id="054fa-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="054fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="054fa-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="054fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="054fa-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="054fa-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="054fa-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="054fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="054fa-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="054fa-115">Not supported.</span></span>|
|<span data-ttu-id="054fa-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="054fa-116">Application</span></span>|<span data-ttu-id="054fa-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="054fa-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="054fa-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="054fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="054fa-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="054fa-119">Request headers</span></span>
|<span data-ttu-id="054fa-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="054fa-120">Header</span></span>|<span data-ttu-id="054fa-121">Значение</span><span class="sxs-lookup"><span data-stu-id="054fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="054fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="054fa-122">Authorization</span></span>|<span data-ttu-id="054fa-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="054fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="054fa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="054fa-124">Accept</span></span>|<span data-ttu-id="054fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="054fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="054fa-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="054fa-126">Request body</span></span>
<span data-ttu-id="054fa-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="054fa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="054fa-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="054fa-128">Response</span></span>
<span data-ttu-id="054fa-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="054fa-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="054fa-130">Пример</span><span class="sxs-lookup"><span data-stu-id="054fa-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="054fa-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="054fa-131">Request</span></span>
<span data-ttu-id="054fa-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="054fa-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="054fa-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="054fa-133">Response</span></span>
<span data-ttu-id="054fa-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="054fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




