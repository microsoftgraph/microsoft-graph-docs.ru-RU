---
title: Список Виндовсаутопилотдеплойментпрофилеассигнментс
description: Список свойств и связей объектов Виндовсаутопилотдеплойментпрофилеассигнмент.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 85e487302608e21df01986d253a5e01f8d5eb4dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980886"
---
# <a name="list-windowsautopilotdeploymentprofileassignments"></a><span data-ttu-id="1adea-103">Список Виндовсаутопилотдеплойментпрофилеассигнментс</span><span class="sxs-lookup"><span data-stu-id="1adea-103">List windowsAutopilotDeploymentProfileAssignments</span></span>

> <span data-ttu-id="1adea-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1adea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1adea-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1adea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1adea-106">Список свойств и связей объектов [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="1adea-106">List properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1adea-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1adea-107">Prerequisites</span></span>
<span data-ttu-id="1adea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1adea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1adea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1adea-110">Permission type</span></span>|<span data-ttu-id="1adea-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1adea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1adea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1adea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1adea-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1adea-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1adea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1adea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1adea-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1adea-115">Not supported.</span></span>|
|<span data-ttu-id="1adea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1adea-116">Application</span></span>|<span data-ttu-id="1adea-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1adea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1adea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1adea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1adea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1adea-119">Request headers</span></span>
|<span data-ttu-id="1adea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1adea-120">Header</span></span>|<span data-ttu-id="1adea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1adea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1adea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1adea-122">Authorization</span></span>|<span data-ttu-id="1adea-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1adea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1adea-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1adea-124">Accept</span></span>|<span data-ttu-id="1adea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1adea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1adea-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1adea-126">Request body</span></span>
<span data-ttu-id="1adea-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1adea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1adea-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="1adea-128">Response</span></span>
<span data-ttu-id="1adea-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1adea-129">If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1adea-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1adea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1adea-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1adea-131">Request</span></span>
<span data-ttu-id="1adea-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1adea-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments
```

### <a name="response"></a><span data-ttu-id="1adea-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1adea-133">Response</span></span>
<span data-ttu-id="1adea-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1adea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
      "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





