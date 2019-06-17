---
title: Действие assign
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a195ac42bbd020775493c218da34369ad2b2c53
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981610"
---
# <a name="assign-action"></a><span data-ttu-id="3b835-103">Действие назначения</span><span class="sxs-lookup"><span data-stu-id="3b835-103">assign action</span></span>

> <span data-ttu-id="3b835-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b835-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b835-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b835-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b835-106">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="3b835-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b835-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3b835-107">Prerequisites</span></span>
<span data-ttu-id="3b835-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b835-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b835-110">Permission type</span></span>|<span data-ttu-id="3b835-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b835-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b835-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b835-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b835-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b835-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3b835-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b835-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b835-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b835-115">Not supported.</span></span>|
|<span data-ttu-id="3b835-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3b835-116">Application</span></span>|<span data-ttu-id="3b835-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b835-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b835-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b835-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assign
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile/assign
```

## <a name="request-headers"></a><span data-ttu-id="3b835-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3b835-119">Request headers</span></span>
|<span data-ttu-id="3b835-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b835-120">Header</span></span>|<span data-ttu-id="3b835-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3b835-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b835-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3b835-122">Authorization</span></span>|<span data-ttu-id="3b835-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b835-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b835-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3b835-124">Accept</span></span>|<span data-ttu-id="3b835-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b835-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b835-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3b835-126">Request body</span></span>
<span data-ttu-id="3b835-127">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b835-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3b835-128">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="3b835-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3b835-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b835-129">Property</span></span>|<span data-ttu-id="3b835-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3b835-130">Type</span></span>|<span data-ttu-id="3b835-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3b835-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b835-132">Девицеидс</span><span class="sxs-lookup"><span data-stu-id="3b835-132">deviceIds</span></span>|<span data-ttu-id="3b835-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3b835-133">String collection</span></span>|<span data-ttu-id="3b835-134">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3b835-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3b835-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="3b835-135">Response</span></span>
<span data-ttu-id="3b835-136">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3b835-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b835-137">Пример</span><span class="sxs-lookup"><span data-stu-id="3b835-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b835-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b835-138">Request</span></span>
<span data-ttu-id="3b835-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b835-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assign

Content-type: application/json
Content-length: 51

{
  "deviceIds": [
    "Device Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3b835-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b835-140">Response</span></span>
<span data-ttu-id="3b835-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b835-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





