---
title: Получение Виндовсаутопилотдеплойментпрофилеассигнмент
description: Чтение свойств и связей объекта Виндовсаутопилотдеплойментпрофилеассигнмент.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb1894dc727ab8a38ca09a5acdc10a23ad4e0c49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150227"
---
# <a name="get-windowsautopilotdeploymentprofileassignment"></a><span data-ttu-id="eedec-103">Получение Виндовсаутопилотдеплойментпрофилеассигнмент</span><span class="sxs-lookup"><span data-stu-id="eedec-103">Get windowsAutopilotDeploymentProfileAssignment</span></span>

> <span data-ttu-id="eedec-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eedec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eedec-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eedec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eedec-106">Чтение свойств и связей объекта [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="eedec-106">Read properties and relationships of the [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eedec-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="eedec-107">Prerequisites</span></span>
<span data-ttu-id="eedec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="eedec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eedec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eedec-110">Permission type</span></span>|<span data-ttu-id="eedec-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="eedec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eedec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eedec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eedec-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="eedec-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="eedec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eedec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eedec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eedec-115">Not supported.</span></span>|
|<span data-ttu-id="eedec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eedec-116">Application</span></span>|<span data-ttu-id="eedec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eedec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eedec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eedec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="eedec-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="eedec-119">Optional query parameters</span></span>
<span data-ttu-id="eedec-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="eedec-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eedec-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eedec-121">Request headers</span></span>
|<span data-ttu-id="eedec-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eedec-122">Header</span></span>|<span data-ttu-id="eedec-123">Значение</span><span class="sxs-lookup"><span data-stu-id="eedec-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eedec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="eedec-124">Authorization</span></span>|<span data-ttu-id="eedec-125">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="eedec-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eedec-126">Accept</span><span class="sxs-lookup"><span data-stu-id="eedec-126">Accept</span></span>|<span data-ttu-id="eedec-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eedec-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eedec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eedec-128">Request body</span></span>
<span data-ttu-id="eedec-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eedec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eedec-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="eedec-130">Response</span></span>
<span data-ttu-id="eedec-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [виндовсаутопилотдеплойментпрофилеассигнмент](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eedec-131">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eedec-132">Пример</span><span class="sxs-lookup"><span data-stu-id="eedec-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="eedec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="eedec-133">Request</span></span>
<span data-ttu-id="eedec-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eedec-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignments/{windowsAutopilotDeploymentProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="eedec-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="eedec-135">Response</span></span>
<span data-ttu-id="eedec-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="eedec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfileAssignment",
    "id": "de7e1e1e-1e1e-de7e-1e1e-7ede1e1e7ede",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




