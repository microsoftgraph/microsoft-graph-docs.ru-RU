---
title: Получение Виндовсаутопилотдеплойментпрофилеассигнмент
description: Чтение свойств и связей объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d12cdf3c27ee3b9227e3f652999ac6a97c0f5cc7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42805068"
---
# <a name="get-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="abb92-103">Получение Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="abb92-103">Get windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="abb92-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb92-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abb92-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="abb92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abb92-106">Чтение свойств и связей объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="abb92-106">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abb92-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="abb92-107">Prerequisites</span></span>
<span data-ttu-id="abb92-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abb92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abb92-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abb92-110">Permission type</span></span>|<span data-ttu-id="abb92-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="abb92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abb92-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abb92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abb92-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb92-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="abb92-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abb92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abb92-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abb92-115">Not supported.</span></span>|
|<span data-ttu-id="abb92-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="abb92-116">Application</span></span>|<span data-ttu-id="abb92-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="abb92-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="abb92-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abb92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abb92-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abb92-119">Optional query parameters</span></span>
<span data-ttu-id="abb92-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="abb92-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abb92-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abb92-121">Request headers</span></span>
|<span data-ttu-id="abb92-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abb92-122">Header</span></span>|<span data-ttu-id="abb92-123">Значение</span><span class="sxs-lookup"><span data-stu-id="abb92-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abb92-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="abb92-124">Authorization</span></span>|<span data-ttu-id="abb92-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abb92-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abb92-126">Accept</span><span class="sxs-lookup"><span data-stu-id="abb92-126">Accept</span></span>|<span data-ttu-id="abb92-127">application/json</span><span class="sxs-lookup"><span data-stu-id="abb92-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abb92-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abb92-128">Request body</span></span>
<span data-ttu-id="abb92-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abb92-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abb92-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="abb92-130">Response</span></span>
<span data-ttu-id="abb92-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="abb92-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abb92-132">Пример</span><span class="sxs-lookup"><span data-stu-id="abb92-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="abb92-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="abb92-133">Request</span></span>
<span data-ttu-id="abb92-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abb92-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="abb92-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="abb92-135">Response</span></span>
<span data-ttu-id="abb92-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="abb92-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
    "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```




